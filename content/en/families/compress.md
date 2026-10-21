---
title: "Compression, delta & erasure"
weight: 130
---

# Compression, delta & erasure {#compression-delta-erasure}

Making bytes smaller, sending only what changed, and surviving what is lost.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-compressions`](https://github.com/go-compressions) | 13 | [site](https://go-compressions.github.io/) | [docs](https://go-compressions.github.io/docs/) | The codecs and the halves of them that are missing elsewhere: LZFSE, LZ4 and DEFLATE wire-compatible with compress/flate both ways, a bzip2 encoder the standard library does not have, and readers for the formats it never grew — .Z, lzip, LZO1X — plus BLAKE3 and b3sum, and the CLIs that go with them. Correctness is judged against the thing itself: the official BLAKE3 vectors, compress/bzip2, and macOS's own libcompression asked what the bytes should be. |
| [`go-deltasync`](https://github.com/go-deltasync) | 6 | [site](https://go-deltasync.github.io/) | [docs](https://go-deltasync.github.io/docs/) | Delta transfer: zsync2, rdiff, zchunk, vcdiff, bita — and the one content-defined chunker they all import. |
| [`go-erasure`](https://github.com/go-erasure) | 2 | [site](https://go-erasure.github.io/) | [docs](https://go-erasure.github.io/docs/) | Erasure coding: Reed-Solomon over GF(2^16), and the Mojette transform. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
