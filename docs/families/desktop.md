# Desktop & widgets

One widget toolkit, every surface it paints on, and the platform plumbing a real desktop needs.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-widgets`](https://github.com/go-widgets) | 16 | [site](https://go-widgets.github.io/) | — | The widget toolkit and every surface it paints on: the painter seam, MVVM, a declarative skin engine, a terminal back-end, a native window on X11, Wayland, Cocoa and Win32, a real Android APK, and a desktop shell. |
| [`go-freedesktop`](https://github.com/go-freedesktop) | 8 | [site](https://go-freedesktop.github.io/) | [docs](https://go-freedesktop.github.io/docs/) | freedesktop.org integration — .desktop entries, icon themes, shared MIME info, application associations, the menu tree, desktop notifications and Secret Service. |
| [`go-iconoir`](https://github.com/go-iconoir) | 1 | [site](https://go-iconoir.github.io/) | — | The whole Iconoir set — 1,671 SVGs embedded and rendered to anti-aliased coverage masks for the toolkit painter. |
| [`go-thumbnail`](https://github.com/go-thumbnail) | 1 | [site](https://go-thumbnail.github.io/) | [docs](https://go-thumbnail.github.io/docs/) | The freedesktop Thumbnail Managing Standard cache. |
| [`go-keyring`](https://github.com/go-keyring) | 1 | [site](https://go-keyring.github.io/) | — | One secret store over macOS Keychain, Windows Credential Manager and Linux Secret Service — no cgo, no CLI exec. |
| [`go-macos`](https://github.com/go-macos) | 6 | [site](https://go-macos.github.io/) | — | The macOS foundation: the shared Objective-C runtime bridge over purego, plus Keychain and notifications. |
| [`go-mswin`](https://github.com/go-mswin) | 2 | [site](https://go-mswin.github.io/) | — | The Windows foundation: Win32 bindings and WinRT interop on combase — peer of go-macos/objc. |
| [`wasmdesk`](https://github.com/wasmdesk) | 7 | [site](https://wasmdesk.github.io/) | — | A desktop in the browser — a Wayland-inspired compositor and window manager, a dock, a login portal, OCI app packaging and a coreutils suite. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
