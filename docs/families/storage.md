# Storage, volumes & filesystems

From a block device to a mounted filesystem, without a C library anywhere.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-volumes`](https://github.com/go-volumes) | 9 | [site](https://go-volumes.github.io/) | [docs](https://go-volumes.github.io/docs/) | The block layer — a device contract, NBD, pools, replicas, S3, an OCI image as a block device, GPT and MBR, and parse-hardening guards. |
| [`go-filesystems`](https://github.com/go-filesystems) | 17 | [site](https://go-filesystems.github.io/) | [docs](https://go-filesystems.github.io/docs/) | Filesystem-format drivers — ext4, xfs, btrfs, zfs, apfs, ntfs, exfat, fat32, iso9660, squashfs and more — plus UEFI variable management and a format prober. |
| [`go-diskimages`](https://github.com/go-diskimages) | 6 | [site](https://go-diskimages.github.io/) | [docs](https://go-diskimages.github.io/docs/) | Disk-image formats: qcow2, raw, dmg, tart-oci, in either direction. |
| [`go-fsctl`](https://github.com/go-fsctl) | 6 | [site](https://go-fsctl.github.io/) | [docs](https://go-fsctl.github.io/docs/) | Linux kernel ioctl wrappers — zfs, btrfs, loop, device-mapper, block, copy-on-write clones. |
| [`go-fde`](https://github.com/go-fde) | 4 | [site](https://go-fde.github.io/) | [docs](https://go-fde.github.io/docs/) | Full-disk encryption: LUKS, APFS, and the plumbing that opens them. |
| [`go-encryptions`](https://github.com/go-encryptions) | 3 | [site](https://go-encryptions.github.io/) | [docs](https://go-encryptions.github.io/docs/) | The modes underneath: CCM, XTS, ZFS crypto. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
