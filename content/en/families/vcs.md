---
title: "Version control & forges"
weight: 180
---

# Version control & forges {#version-control-forges}

Hosting Git itself: the wire protocol underneath, the forge around it, and the CI that runs on it.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-vcs`](https://github.com/go-vcs) | 4 | [site](https://go-vcs.github.io/) | [docs](https://go-vcs.github.io/docs/) | A light, secure Git forge — hosting, web UI, admin gRPC, Actions runners through GARM — standing on an owned implementation of the Git wire protocol v2 and pack files, fuzzed and measured against git itself, with a workflow engine that speaks the gitea-runner protocol and a local agent-facing daemon. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
