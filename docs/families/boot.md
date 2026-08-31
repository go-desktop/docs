# Firmware, boot & trust

What runs before the kernel, and how you prove what ran.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-tpm2`](https://github.com/go-tpm2) | 8 | [site](https://go-tpm2.github.io/) | [docs](https://go-tpm2.github.io/docs/) | TPM 2.0 end to end: transports, the command layer, EFI_TCG2, measured boot, event-log replay and remote attestation. |
| [`go-coff`](https://github.com/go-coff) | 4 | [site](https://go-coff.github.io/) | [docs](https://go-coff.github.io/docs/) | PE/COFF for UEFI — an object-to-EFI linker, a signing and conversion CLI, and a self-extracting EFI packer. |
| [`go-bootloaders`](https://github.com/go-bootloaders) | 2 | [site](https://go-bootloaders.github.io/) | [docs](https://go-bootloaders.github.io/docs/) | GRUB and systemd-boot tooling, composed on the storage, UEFI and TPM stacks rather than reimplementing them. |
| [`cloud-boot`](https://github.com/cloud-boot) | 7 | [site](https://cloud-boot.github.io/) | [docs](https://cloud-boot.github.io/docs/) | Booting the machine: a TamaGo UEFI payload, a unified kernel image, an init, kernels, ISOs, SEV-SNP. |
| [`nano-container-linux`](https://github.com/nano-container-linux) | 7 | [site](https://nano-container-linux.github.io/) | [docs](https://nano-container-linux.github.io/docs/) | A minimal container host — OCI initrd and PXE boot, a DNS daemon, an OpenPubKey agent. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
