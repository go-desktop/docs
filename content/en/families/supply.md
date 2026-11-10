---
title: "Packaging & supply chain"
weight: 160
---

# Packaging & supply chain {#packaging-supply-chain}

Building every dependency from source, signing it, and saying where it came from.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-zpkg`](https://github.com/go-zpkg) | 8 | [site](https://go-zpkg.github.io/) | [docs](https://go-zpkg.github.io/docs/) | A pure-Go package manager: the installer, the bottle builder, the recipe builder, and the CI factory that publishes signed bottles. Formerly go-pkgx; the organisation was renamed and its repositories transferred, so `pkgx` became `zpkgx` and the store moved from ~/.pkgx to ~/.zpkg. |
| [`go-attest`](https://github.com/go-attest) | 2 | [site](https://go-attest.github.io/) | [docs](https://go-attest.github.io/docs/) | SPDX and CycloneDX SBOMs, SLSA provenance, and Ed25519 signing that is minisign- and cosign-interoperable from one keypair. |
| [`go-versions`](https://github.com/go-versions) | 1 | [site](https://go-versions.github.io/) | [docs](https://go-versions.github.io/docs/) | Loose, pkgx-compatible semantic versions and ranges, CalVer included. |
| [`go-gitsafe`](https://github.com/go-gitsafe) | 1 | [site](https://go-gitsafe.github.io/) | [docs](https://go-gitsafe.github.io/docs/) | Guards on what leaves a machine: a global git hook that refuses a credential in a remote URL and a write to the branch pull requests land on, a credential helper that never lets a token reach a command line, and a scope checker that reads a token's powers without printing it. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
