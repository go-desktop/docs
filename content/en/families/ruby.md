---
title: "Languages, in Go"
weight: 110
---

# Languages, in Go {#languages-in-go}

Other languages' runtimes, written in pure Go so they embed in a Go program and compile to WebAssembly: a Ruby virtual machine with one organisation per gem it needs, and interpreters for Julia, R and C.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-embedded-ruby`](https://github.com/go-embedded-ruby) | 1 | [site](https://go-embedded-ruby.github.io/) | [docs](https://go-embedded-ruby.github.io/docs/) | The Ruby virtual machine — YARV bytecode, the object model, the core library, and the rbgo interpreter. |
| [`go-embedded-julia`](https://github.com/go-embedded-julia) | 1 | [site](https://go-embedded-julia.github.io/) | [docs](https://go-embedded-julia.github.io/docs/) | A Julia interpreter in pure Go, embeddable and WebAssembly-ready. |
| [`go-embedded-r`](https://github.com/go-embedded-r) | 2 | [site](https://go-embedded-r.github.io/) | [docs](https://go-embedded-r.github.io/docs/) | An embeddable R interpreter in pure Go, checked against GNU R 4.6.2 by an oracle harness rather than against itself. |
| [`go-embedded-c`](https://github.com/go-embedded-c) | 1 | — | — | C in pure Go: an oracle harness and a C-to-wasm32 compiler, so a notebook cell can hold C. |
| [`go-composites`](https://github.com/go-composites) | 31 | [site](https://go-composites.github.io/) | [docs](https://go-composites.github.io/docs/) | Ruby's numeric tower, collections, time and dates as composition-oriented building blocks: Result-based, Null-Object, never nil. |
| [`go-ruby-widgets`](https://github.com/go-ruby-widgets) | 3 | [site](https://go-ruby-widgets.github.io/) | [docs](https://go-ruby-widgets.github.io/docs/) | MVVM, widgets and a terminal toolkit, addressable from Ruby. |
| [`go-vet-analyzers`](https://github.com/go-vet-analyzers) | 2 | [site](https://go-vet-analyzers.github.io/) | [docs](https://go-vet-analyzers.github.io/docs/) | go vet analyzers that make the ecosystem's invariants a compile-time matter. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
