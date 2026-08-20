# What every repository is held to

The same conformance standard applies across all 287 organisations. That is what
makes them one ecosystem rather than a pile of unrelated modules: a caller can
assume the same things about any of them without reading its CI configuration.

## `CGO_ENABLED=0`

No cgo, and no shelling out to a command-line tool in place of a library. A
dependency is a Go module or it is written.

The rule is stricter than it first sounds, because `exec.Command` to a CLI is the
usual way a cgo dependency comes back in disguise — the binary is still C, it is
just C the build no longer sees. A library that runs `mkfs.ext4` has not removed
the C dependency; it has removed the compiler's knowledge of it.

What the rule buys, concretely: cross-compilation to six architectures from one
machine, a `js/wasm` build that runs the *same* code in a browser tab, and a
bare-metal target with no libc underneath.

## Six 64-bit targets

Build and test on **amd64, arm64, riscv64, loong64, ppc64le and s390x** — native
where runners exist, under qemu-user (Debian trixie, per-architecture `QEMU_CPU`)
otherwise.

s390x earns its place by being big-endian. Any on-disk or on-wire encoding that
was quietly written little-endian-first fails there and nowhere else, which is
exactly the bug that is invisible on a developer's machine and fatal in a file
format.

## 100% statement coverage

A CI gate, error branches included.

Two clarifications that matter more than the number:

- **A skipped test is not a passing one.** Jobs fail when a toolchain or a device
  is missing, rather than turning green with the interesting case unexecuted. A
  green run whose `-run` filter matched nothing is worse than a red one, because
  it is believed.
- **Coverage is measured the way CI measures it** — with `-coverpkg` over the
  packages under test, not per-package defaults that can report 100% while leaving
  a package unexercised.

## Measured, not asserted

A performance claim comes with a benchmark against the reference implementation —
MRI for the Ruby stack, the C library for a codec, numpy or scipy for a numeric
kernel. A claim that an implementation is faithful to a format comes with a byte
comparison against that reference, not a round-trip through itself.

Decoders are fuzzed. On the filesystem drivers, 70 million executions found two
denial-of-service panics that no hand-written test had reached.

Where a claim is about something that runs — a window opening, a widget drawing,
a page rendering — it is verified by capture, not by reasoning about the code.

## Reference libraries first

Where a good pure-Go library already exists, it is used rather than rewritten. The
ecosystem is large because a great many capabilities had no pure-Go
implementation, not because everything was rebuilt on principle — and one
organisation in it has already been retired for duplicating a reference library
that was itself CGO-free.

## One landing, one docs site

Each organisation publishes a Hugo landing page at `<org>.github.io` and versioned
MkDocs Material documentation at `<org>.github.io/docs/`, with the same brand,
an 88-pixel hero logo, a favicon, and a light/dark/system theme toggle that
defaults to system.

## BSD-3-Clause

Every repository, every organisation. Copyright is held by the authors of the
organisation the code lives in.

## Go 1.26.4 floor

New repositories set the `go` directive to `1.26.4` — the full patch version, not
a bare `1.26`. A low `go` directive is never deliberate; where one is found it is
a drift to fix, not a compatibility decision to respect.
