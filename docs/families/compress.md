# Compression, delta & erasure

Making bytes smaller, sending only what changed, and surviving what is lost.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-compressions`](https://github.com/go-compressions) | 8 | [site](https://go-compressions.github.io/) | [docs](https://go-compressions.github.io/docs/) | LZFSE, LZ4, deflate and BLAKE3, with the CLIs that go with them. |
| [`go-deltasync`](https://github.com/go-deltasync) | 6 | [site](https://go-deltasync.github.io/) | [docs](https://go-deltasync.github.io/docs/) | Delta transfer: zsync2, rdiff, zchunk, vcdiff, bita — and the one content-defined chunker they all import. |
| [`go-erasure`](https://github.com/go-erasure) | 2 | [site](https://go-erasure.github.io/) | [docs](https://go-erasure.github.io/docs/) | Erasure coding: Reed-Solomon over GF(2^16), and the Mojette transform. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
