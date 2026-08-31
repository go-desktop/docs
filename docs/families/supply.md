# Packaging & supply chain

Building every dependency from source, signing it, and saying where it came from.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-pkgx`](https://github.com/go-pkgx) | 8 | [site](https://go-pkgx.github.io/) | [docs](https://go-pkgx.github.io/docs/) | A pure-Go pkgx: the package manager, the bottle installer, the bk recipe builder, and the CI factory that publishes signed bottles. |
| [`go-attest`](https://github.com/go-attest) | 2 | [site](https://go-attest.github.io/) | [docs](https://go-attest.github.io/docs/) | SPDX and CycloneDX SBOMs, SLSA provenance, and Ed25519 signing that is minisign- and cosign-interoperable from one keypair. |
| [`go-versions`](https://github.com/go-versions) | 1 | [site](https://go-versions.github.io/) | [docs](https://go-versions.github.io/docs/) | Loose, pkgx-compatible semantic versions and ranges, CalVer included. |
| [`go-gitsafe`](https://github.com/go-gitsafe) | 1 | — | — | Guards on what leaves a machine: a global git hook that refuses a credential in a remote URL and a write to the branch pull requests land on, a credential helper that never lets a token reach a command line, and a scope checker that reads a token's powers without printing it. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
