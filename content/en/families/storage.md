---
title: "Storage, volumes & filesystems"
weight: 140
---

# Storage, volumes & filesystems {#storage-volumes-filesystems}

From a block device to a mounted filesystem, without a C library anywhere.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-volumes`](https://github.com/go-volumes) | 9 | [site](https://go-volumes.github.io/) | [docs](https://go-volumes.github.io/docs/) | The block layer — a device contract, NBD, pools, replicas, S3, an OCI image as a block device, GPT and MBR, and parse-hardening guards. |
| [`go-filesystems`](https://github.com/go-filesystems) | 34 | [site](https://go-filesystems.github.io/) | [docs](https://go-filesystems.github.io/docs/) | One Filesystem interface, and everything that can sit on either side of it. Underneath, the formats: ext4, xfs, btrfs, zfs, apfs, ntfs, exfat, fat32, ffs, ufs, hfsplus, iso9660, squashfs, UEFI variables, a blkid-style prober — and archives read as filesystems rather than unpacked, cab, cpio, rar, rpm, 7z (which also writes), xar and WARC, with one extractor that sniffs the format from the bytes and follows multi-volume sets. Above it, the servers that export any of them — NFSv3, SMB2, SFTP, WebDAV and an S3 object API — so an image is mounted by the host instead of only read by a program. And between the two: a host directory confined with os.Root, a read-only filesystem made writable through a spool, and the same filesystem served across a connection. |
| [`go-diskimages`](https://github.com/go-diskimages) | 6 | [site](https://go-diskimages.github.io/) | [docs](https://go-diskimages.github.io/docs/) | Disk-image formats: qcow2, raw, dmg, tart-oci, in either direction. |
| [`go-fileshare`](https://github.com/go-fileshare) | 4 | [site](https://go-fileshare.github.io/) | [docs](https://go-fileshare.github.io/docs/) | The product go-filesystems' servers make possible: one configuration and one binary sharing a disk image over SMB, NFS, WebDAV and SFTP, with an OIDC portal, per-server tokens, a file explorer and an admin console across many servers. |
| [`go-fsctl`](https://github.com/go-fsctl) | 7 | [site](https://go-fsctl.github.io/) | [docs](https://go-fsctl.github.io/docs/) | Linux kernel ioctl wrappers — zfs, btrfs, loop, device-mapper, block, copy-on-write clones. |
| [`go-fde`](https://github.com/go-fde) | 4 | [site](https://go-fde.github.io/) | [docs](https://go-fde.github.io/docs/) | Full-disk encryption: LUKS, APFS, and the plumbing that opens them. |
| [`go-encryptions`](https://github.com/go-encryptions) | 4 | [site](https://go-encryptions.github.io/) | [docs](https://go-encryptions.github.io/docs/) | The modes underneath: CCM, XTS, ZFS crypto. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
