---
title: "Documents, typesetting & fonts"
weight: 70
---

# Documents, typesetting & fonts {#documents-typesetting-fonts}

Turning a document into pages: fonts, breaking, shaping, TeX, PDF, and one rich-document model.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-tex`](https://github.com/go-tex) | 5 | [site](https://go-tex.github.io/) | [docs](https://go-tex.github.io/docs/) | A TeX engine — mouth and gullet, math mode to SVG, a PDF-figure rasteriser, and a fetcher that gets a document the class files it asks for without redistributing any. |
| [`go-typeset`](https://github.com/go-typeset) | 3 | [site](https://go-typeset.github.io/) | [docs](https://go-typeset.github.io/docs/) | The typesetting algorithms on their own, with no TeX vocabulary in the API: Knuth-Plass line breaking, Liang hyphenation, the Unicode bidirectional algorithm. |
| [`go-opentype`](https://github.com/go-opentype) | 3 | [site](https://go-opentype.github.io/) | [docs](https://go-opentype.github.io/docs/) | The font format: TrueType/OpenType parsing and anti-aliased rasterisation, a HarfBuzz-lite complex-text shaper, and legible fonts ready to import. |
| [`go-synctex`](https://github.com/go-synctex) | 1 | [site](https://go-synctex.github.io/) | [docs](https://go-synctex.github.io/docs/) | TeX's SyncTeX — the source-to-PDF correspondence, both ways. |
| [`go-pdfkit`](https://github.com/go-pdfkit) | 15 | [site](https://go-pdfkit.github.io/) | [docs](https://go-pdfkit.github.io/docs/) | The PDF stack, both directions: a 1.7 writer with TrueType and CFF subsetting, a reader and renderer, AcroForm and XFA form fields, text and structure extraction, a conformance suite judged against poppler, and a co-editable reader application built on all of it. |
| [`go-docutils`](https://github.com/go-docutils) | 2 | [site](https://go-docutils.github.io/) | [docs](https://go-docutils.github.io/docs/) | reStructuredText both ways: docutils' core in pure Go — the parser and the doctree the LaTeX and PDF path is built on — and an extractor that renders a Go package's own API documentation as reST to feed it. |
| [`go-richdoc`](https://github.com/go-richdoc) | 10 | [site](https://go-richdoc.github.io/) | [docs](https://go-richdoc.github.io/docs/) | One rich-document model, and the converters that read and write it — Markdown, LaTeX and reStructuredText. |
| [`go-odf`](https://github.com/go-odf) | 1 | [site](https://go-odf.github.io/) | [docs](https://go-odf.github.io/docs/) | OpenDocument Text, in and out of the richdoc model. |
| [`go-rtf`](https://github.com/go-rtf) | 1 | [site](https://go-rtf.github.io/) | [docs](https://go-rtf.github.io/docs/) | RTF, in and out of the richdoc model. |
| [`go-ooxml`](https://github.com/go-ooxml) | 2 | [site](https://go-ooxml.github.io/) | — | Word, Excel and PowerPoint into the richdoc model: one container — the Open Packaging Conventions, kept separate because docx, xlsx and pptx all sit on it — and three vocabularies above it. |
| [`go-slides`](https://github.com/go-slides) | 2 | [site](https://go-slides.github.io/) | [docs](https://go-slides.github.io/docs/) | Marp-compatible slide decks, with Go template interpolation and slide kinds, and the VS Code extension that previews and exports them. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
