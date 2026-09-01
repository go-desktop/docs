# Desktop & widgets

One widget toolkit, every surface it paints on, and the platform plumbing a real desktop needs.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-gtk`](https://github.com/go-gtk) | 1 | — | — | GTK4 driven from pure Go over purego, CGO=0 — the Linux native-toolkit bridge for go-widgets, sibling of go-macos/objc. |
| [`go-widgets`](https://github.com/go-widgets) | 19 | [site](https://go-widgets.github.io/) | [docs](https://go-widgets.github.io/docs/) | The widget toolkit and every surface it paints on: the painter seam, MVVM, a declarative skin engine, a terminal back-end, a native window on X11, Wayland, Cocoa and Win32, application lifecycle with a system tray, a real Android APK, and a desktop shell. |
| [`go-freedesktop`](https://github.com/go-freedesktop) | 10 | [site](https://go-freedesktop.github.io/) | [docs](https://go-freedesktop.github.io/docs/) | freedesktop.org integration — .desktop entries, icon themes, shared MIME info, application associations, the menu tree, desktop notifications and Secret Service — over an owned X11 protocol core that also serves screen capture and the toolkit's window back-end. |
| [`go-icons`](https://github.com/go-icons) | 6 | [site](https://go-icons.github.io/) | [docs](https://go-icons.github.io/docs/) | Icon and logo packs as embedded pure-Go SVG data — Simple Icons brand marks, Devicon, Material and Seti file types, vscode-icons, and Iconoir. One repository per pack, so a program embeds the set it draws and not the other five; the drawing itself is go-gfx's `svg` package. |
| [`go-thumbnail`](https://github.com/go-thumbnail) | 1 | [site](https://go-thumbnail.github.io/) | [docs](https://go-thumbnail.github.io/docs/) | The freedesktop Thumbnail Managing Standard cache. |
| [`go-keyring`](https://github.com/go-keyring) | 1 | [site](https://go-keyring.github.io/) | [docs](https://go-keyring.github.io/docs/) | One secret store over macOS Keychain, Windows Credential Manager and Linux Secret Service — no cgo, no CLI exec. |
| [`go-macos`](https://github.com/go-macos) | 26 | [site](https://go-macos.github.io/) | [docs](https://go-macos.github.io/docs/) | The macOS foundation, all of it CGO-free through purego: the shared Objective-C runtime bridge, real AppKit controls embedded in a Go-painted window, Keychain and Touch ID, notifications and menu-bar items, accessibility, global hotkeys, login items and launch agents, IOKit HID, DiskArbitration, hardware audio and video decode, ScreenCaptureKit capture, and virtual displays the desktop extends onto. |
| [`go-mswin`](https://github.com/go-mswin) | 3 | [site](https://go-mswin.github.io/) | [docs](https://go-mswin.github.io/docs/) | The Windows foundation: Win32 bindings and WinRT interop on combase — peer of go-macos/objc — plus DXGI Desktop Duplication and GDI screen capture built on them. |
| [`wasmdesk`](https://github.com/wasmdesk) | 7 | [site](https://wasmdesk.github.io/) | [docs](https://wasmdesk.github.io/docs/) | A desktop in the browser — a Wayland-inspired compositor and window manager, a dock, a login portal, OCI app packaging and a coreutils suite. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
