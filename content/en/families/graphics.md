---
title: "Graphics, images & media"
weight: 60
---

# Graphics, images & media {#graphics-images-media}

The 2D socle everything above draws through, and the pixels and frames it moves.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-gfx`](https://github.com/go-gfx) | 3 | [site](https://go-gfx.github.io/) | [docs](https://go-gfx.github.io/docs/) | The shared 2D socle: an anti-aliased vector rasteriser, a raster surface, colour, geometry, resampling, and SVG to bitmap. |
| [`go-images`](https://github.com/go-images) | 7 | [site](https://go-images.github.io/) | [docs](https://go-images.github.io/docs/) | Image processing at scikit-image scope, plus the decoders the standard library does not have or does differently: Photoshop PSD composites, and forks of image/gif, image/jpeg and image/png that upsample four-component chroma the way libjpeg does and can report what a truncated stream did decode, so a half-arrived picture still shows. And one that is not processing at all: depth from a single photograph, and the second eye synthesised from it. |
| [`go-avkit`](https://github.com/go-avkit) | 7 | [site](https://go-avkit.github.io/) | [docs](https://go-avkit.github.io/docs/) | An audio/video toolkit: MP4/ISO-BMFF, Matroska/WebM and MPEG-TS onto one model, demuxed and muxed — and under it the bitstreams themselves, H.264 and H.265 read down to clause 8.2's picture order counts, VP8 and VP9, over the primitives they share rather than once per codec: RBSP and Exp-Golomb bit reading, NAL framing, and the boolean arithmetic decoder VP8 and VP9 have in common. |
| [`go-streamkit`](https://github.com/go-streamkit) | 1 | [site](https://go-streamkit.github.io/) | [docs](https://go-streamkit.github.io/docs/) | Site-agnostic transport for streaming media: a retrying, rate-limited HTTP client, an HLS parser and an MPEG-DASH manifest reader. |
| [`go-extractors`](https://github.com/go-extractors) | 1 | [site](https://go-extractors.github.io/) | [docs](https://go-extractors.github.io/docs/) | A plugin framework for media extractors — standalone plugin executables answer what is at a URL and what can be downloaded from it. |
| [`go-xrkit`](https://github.com/go-xrkit) | 5 | [site](https://go-xrkit.github.io/) | [docs](https://go-xrkit.github.io/docs/) | XR glasses: head orientation, stereo frame packing, flat, equirectangular and fisheye projection, a 360° screen ribbon, a graded catalogue of what each headset can show — plus a player, a virtual desktop on the ribbon, and Android capture. |
| [`go-viture`](https://github.com/go-viture) | 2 | — | — | The VITURE headsets go-xrkit drives: the Beast and the Luma Ultra, spoken to directly with no vendor library. |
| [`go-xreal`](https://github.com/go-xreal) | 1 | — | — | The XREAL Air family's USB packet protocol, the other half of what go-xrkit reads head orientation from. |
| [`go-videodsp`](https://github.com/go-videodsp) | 1 | — | — | Planar YUV to RGBA, the conversion every video decoder in the map ends with, kept in one place rather than once per codec. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
