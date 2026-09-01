# The pure-Go ecosystem

**293 organisations. 635 public code repositories. No C anywhere.**

`go-desktop` holds no library. It holds the index — a way to find a capability
without already knowing which organisation owns it — and
[the tool](https://github.com/go-desktop/catalog) that generates it, so that no
number on these pages is typed by hand.

Every library in the map is written in Go and compiled with `CGO_ENABLED=0`. That
is not a stylistic preference. It is what makes one binary cross-compile to six
architectures, run inside a browser as WebAssembly, and boot on bare metal without
a libc — three things a single cgo dependency takes away permanently.

## How the map is organised

**One organisation per domain, one repository per capability.** A program that
needs an ext4 reader takes an ext4 reader, not a storage framework. This is why
there are 293 organisations rather than a handful of monorepos: the unit of reuse
is the capability, and a capability that lives in its own module can be depended
on without dragging in the rest of its family.

The consequence to be aware of is that the map itself has to be maintained — which
is what this site is for. Before building anything, look here first: the recurring
failure mode in an ecosystem this wide is rebuilding something that already exists
one organisation over.

## Where to start

- **[Find a capability](finding.md)** — a lookup from what you need to where it lives.
- **[What every repository is held to](standards.md)** — the conformance standard, in full.
- The 17 families, in the navigation on the left.
- **[Ruby gems](gems.md)** — the 195 per-gem organisations, alphabetically.
- **[Held, not yet built](reserved.md)** — the names that are held but hold nothing.

## Reading a count

Every repository count on this site is the number of **public repositories that
hold code**. The four infrastructure repositories every organisation carries —
`.github`, `brand`, `docs` and `<org>.github.io` — are excluded, because counting
them would inflate a one-library organisation to five.

Counts were measured against the live GitHub organisation list rather than
recalled, and the generated pages carry no hand-typed numbers.
