# Documents, typesetting & fonts

Turning a document into pages: fonts, breaking, shaping, TeX, PDF, and one rich-document model.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-tex`](https://github.com/go-tex) | 5 | [site](https://go-tex.github.io/) | [docs](https://go-tex.github.io/docs/) | A TeX engine — mouth and gullet, math mode to SVG, a PDF-figure rasteriser, and a fetcher that gets a document the class files it asks for without redistributing any. |
| [`go-typeset`](https://github.com/go-typeset) | 3 | [site](https://go-typeset.github.io/) | — | The typesetting algorithms on their own, with no TeX vocabulary in the API: Knuth-Plass line breaking, Liang hyphenation, the Unicode bidirectional algorithm. |
| [`go-opentype`](https://github.com/go-opentype) | 3 | [site](https://go-opentype.github.io/) | [docs](https://go-opentype.github.io/docs/) | The font format: TrueType/OpenType parsing and anti-aliased rasterisation, a HarfBuzz-lite complex-text shaper, and legible fonts ready to import. |
| [`go-synctex`](https://github.com/go-synctex) | 1 | [site](https://go-synctex.github.io/) | [docs](https://go-synctex.github.io/docs/) | TeX's SyncTeX — the source-to-PDF correspondence, both ways. |
| [`go-pdfkit`](https://github.com/go-pdfkit) | 1 | [site](https://go-pdfkit.github.io/) | [docs](https://go-pdfkit.github.io/docs/) | A PDF 1.7 writer: font subsetting and embedding for TrueType and CFF, graphics, images, shaped text. |
| [`go-richdoc`](https://github.com/go-richdoc) | 3 | — | — | One rich-document model, and the converters that read and write it. |
| [`go-odf`](https://github.com/go-odf) | 1 | — | — | OpenDocument Text, in and out of the richdoc model. |
| [`go-rtf`](https://github.com/go-rtf) | 1 | — | — | RTF, in and out of the richdoc model. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
