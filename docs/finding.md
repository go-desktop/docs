# Find a capability

The ecosystem is wide enough that the real risk is not *finding* a library but
*not knowing it exists* and rebuilding it. This page is the lookup: what you need,
and the module that already does it.

If what you need is not here, check the family pages before starting — and if it
genuinely is not in the ecosystem, it belongs in the organisation that owns the
domain, not in the repository that happens to need it first.

## User interface

| I need to… | Use |
| --- | --- |
| Build a GUI | [`go-widgets/toolkit`](https://github.com/go-widgets/toolkit) |
| Open a real window on Linux, macOS or Windows | [`go-widgets/window`](https://github.com/go-widgets/window) |
| Draw into a terminal instead | [`go-widgets/tui`](https://github.com/go-widgets/tui) |
| Bind state to widgets | [`go-widgets/mvvm`](https://github.com/go-widgets/mvvm) + [`go-widgets/mvvmtk`](https://github.com/go-widgets/mvvmtk) |
| Theme a UI declaratively | [`go-widgets/skin`](https://github.com/go-widgets/skin) |
| Put an icon on a button | [`go-iconoir/iconoir`](https://github.com/go-iconoir/iconoir) — never hand-draw one |
| Highlight source code in an editor widget | [`go-rouge/rouge`](https://github.com/go-rouge/rouge) via `go-widgets/toolkit/rougelex` |
| Add a system-tray or menu-bar item | [`go-widgets/tray`](https://github.com/go-widgets/tray) |
| Animate a widget | `go-widgets/toolkit/anim` |
| Ship an Android APK with a Go-painted UI | [`go-widgets/android`](https://github.com/go-widgets/android) |

## Desktop integration

| I need to… | Use |
| --- | --- |
| Read `.desktop` entries or find installed apps | [`go-freedesktop/desktopentry`](https://github.com/go-freedesktop/desktopentry) |
| Look up an icon by name in the icon theme | [`go-freedesktop/icontheme`](https://github.com/go-freedesktop/icontheme) |
| Detect a file's MIME type | [`go-freedesktop/mime`](https://github.com/go-freedesktop/mime) |
| Find which app opens a type | [`go-freedesktop/mimeapps`](https://github.com/go-freedesktop/mimeapps) |
| Send a desktop notification | [`go-freedesktop/notifications`](https://github.com/go-freedesktop/notifications) |
| Cache a thumbnail | [`go-thumbnail/thumbnail`](https://github.com/go-thumbnail/thumbnail) |
| Store a secret in the OS keychain | [`go-keyring/keyring`](https://github.com/go-keyring/keyring) |
| Talk to D-Bus | `github.com/godbus/dbus/v5` — the reference library, itself CGO-free |
| Call an Objective-C API on macOS | [`go-macos/objc`](https://github.com/go-macos/objc) |
| Call a Win32 or WinRT API | [`go-mswin/win32`](https://github.com/go-mswin/win32), [`go-mswin/winrt`](https://github.com/go-mswin/winrt) |

## Graphics and text

| I need to… | Use |
| --- | --- |
| Fill or stroke a vector path with anti-aliasing | [`go-gfx/gfx`](https://github.com/go-gfx/gfx) (`vector`) |
| Rasterise an SVG to a bitmap | `go-gfx/gfx/svg` |
| Process or transform an image | [`go-images/images`](https://github.com/go-images/images) |
| Parse a font and rasterise glyphs | [`go-opentype/opentype`](https://github.com/go-opentype/opentype) |
| Shape complex text (Arabic, ligatures, marks) | [`go-opentype/shape`](https://github.com/go-opentype/shape) |
| Break a paragraph into lines optimally | [`go-typeset/linebreak`](https://github.com/go-typeset/linebreak) |
| Hyphenate a word | [`go-typeset/hyphenation`](https://github.com/go-typeset/hyphenation) |
| Order bidirectional text | [`go-typeset/bidi`](https://github.com/go-typeset/bidi) |
| Write a PDF | [`go-pdfkit/pdfkit`](https://github.com/go-pdfkit/pdfkit) |
| Typeset TeX, or just TeX math | [`go-tex/engine`](https://github.com/go-tex/engine), [`go-tex/math`](https://github.com/go-tex/math) |
| Get the `.cls`/`.sty` files a document asks for | [`go-tex/texmf`](https://github.com/go-tex/texmf) |
| Demux MP4 or Matroska | [`go-avkit/avkit`](https://github.com/go-avkit/avkit) |

## Documents and markup

| I need to… | Use |
| --- | --- |
| Render CommonMark to HTML | [`go-commonmark/commonmark`](https://github.com/go-commonmark/commonmark) |
| Parse or query HTML and XML | [`go-nokogiri/nokogiri`](https://github.com/go-nokogiri/nokogiri) |
| Compile SCSS | [`go-scss/scss`](https://github.com/go-scss/scss) |
| Render a Liquid or Mustache template | [`go-liquid/liquid`](https://github.com/go-liquid/liquid), [`go-mustache/mustache`](https://github.com/go-mustache/mustache) |
| Match a regex with lookaround or backreferences | [`go-regexp/engine`](https://github.com/go-regexp/engine) — not `regexp2` |
| Convert between rich document formats | [`go-richdoc/richdoc`](https://github.com/go-richdoc/richdoc) and its converters |
| Parse a date a human wrote | [`go-datetime/dates`](https://github.com/go-datetime/dates) |

## Storage and filesystems

| I need to… | Use |
| --- | --- |
| Read a partition table | [`go-volumes/gpt`](https://github.com/go-volumes/gpt) |
| Address a block device, pool, replica or S3 object as one thing | [`go-volumes/interface`](https://github.com/go-volumes/interface) |
| Mount and read ext4, xfs, btrfs, zfs, apfs, ntfs, … | [`go-filesystems`](https://github.com/go-filesystems) — one repository per format |
| Work out what filesystem an image holds | [`go-filesystems/detect`](https://github.com/go-filesystems/detect) |
| Read or write UEFI variables | [`go-filesystems/uefi`](https://github.com/go-filesystems/uefi) |
| Convert a qcow2, raw, dmg or tart-oci image | [`go-diskimages`](https://github.com/go-diskimages) |
| Call a Linux filesystem ioctl | [`go-fsctl`](https://github.com/go-fsctl) |
| Open a LUKS or APFS volume | [`go-fde`](https://github.com/go-fde) |
| Compress with LZ4, LZFSE or deflate | [`go-compressions`](https://github.com/go-compressions) |
| Transfer only what changed | [`go-deltasync`](https://github.com/go-deltasync) |
| Split a stream into content-defined chunks | [`go-deltasync/chunk`](https://github.com/go-deltasync/chunk) — the one chunker |
| Erasure-code data | [`go-erasure/reedsolomon`](https://github.com/go-erasure/reedsolomon) |

## Firmware, boot and trust

| I need to… | Use |
| --- | --- |
| Talk to a TPM, extend a PCR, seal a secret | [`go-tpm2/tpm2`](https://github.com/go-tpm2/tpm2) |
| Replay an event log or verify an attestation | [`go-tpm2/attest`](https://github.com/go-tpm2/attest) |
| Measure into a PCR from UEFI | [`go-tpm2/efitcg2`](https://github.com/go-tpm2/efitcg2) |
| Link or sign a PE32+/EFI binary | [`go-coff/peln`](https://github.com/go-coff/peln), [`go-coff/pectl`](https://github.com/go-coff/pectl) |
| Read or patch GRUB or systemd-boot config | [`go-bootloaders`](https://github.com/go-bootloaders) |

## Compute

| I need to… | Use |
| --- | --- |
| Generate Plan 9 assembly for every 64-bit target | [`go-asmgen/asmgen`](https://github.com/go-asmgen/asmgen) |
| Speed up a codec, hash or string scan with SIMD | [`go-simd`](https://github.com/go-simd) — one repository per kernel |
| Work with n-dimensional arrays, or multiply matrices | [`go-ndarray/ndarray`](https://github.com/go-ndarray/ndarray) |
| Take an FFT | [`go-fft/fft`](https://github.com/go-fft/fft) |

## Distributed systems

| I need to… | Use |
| --- | --- |
| Let many people edit one document | [`go-crdt/crdt`](https://github.com/go-crdt/crdt) + [`go-crdt/collab`](https://github.com/go-crdt/collab) |
| Relay Yjs updates | [`go-yjs-relay/yrelay`](https://github.com/go-yjs-relay/yrelay) |
| Run gRPC over SSH, WireGuard, vsock, WebSocket or WebRTC | [`grpc-transports`](https://github.com/grpc-transports) |
| Elect a leader or watch host liveness | [`go-coord/coord`](https://github.com/go-coord/coord) |
| Supervise processes as PID 1 | [`go-proc/supervisor`](https://github.com/go-proc/supervisor) |
| Serve DHCPv4 | [`go-net-dhcp/dhcp`](https://github.com/go-net-dhcp/dhcp) |
| Health-check a backend | [`go-net-health/health`](https://github.com/go-net-health/health) |
| Drive a guest virtio device | [`go-virtio`](https://github.com/go-virtio) |
| Run a microVM cloud | [`openweft/weft`](https://github.com/openweft/weft) |

## Packaging and Ruby

| I need to… | Use |
| --- | --- |
| Install or build a package from a pkgx recipe | [`go-pkgx/pkgm`](https://github.com/go-pkgx/pkgm), [`go-pkgx/bk`](https://github.com/go-pkgx/bk) |
| Produce an SBOM or sign an artifact | [`go-attest/sbom`](https://github.com/go-attest/sbom), [`go-attest/sign`](https://github.com/go-attest/sign) |
| Compare loose or CalVer versions | [`go-versions/semver`](https://github.com/go-versions/semver) |
| Run Ruby code | [`go-embedded-ruby/ruby`](https://github.com/go-embedded-ruby/ruby) (`rbgo`) |
| Use a specific gem's behaviour from Go | the matching [`go-ruby-*`](gems.md) organisation |
| Compile a Puppet catalogue | [`go-puppet/puppet`](https://github.com/go-puppet/puppet) |
