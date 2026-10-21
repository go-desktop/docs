---
title: "The workshop"
weight: 220
---

# The workshop {#the-workshop}

Tools that act on the ecosystem rather than inside it: they read every repository, and the thing they protect is that a claim made about all of them is measured rather than remembered.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-fleettools`](https://github.com/go-fleettools) | 9 | — | — | Sweeps across the whole map, each answering one question and refusing to answer it vaguely: which default branches are red, which modules declare a toolchain floor below the one a fix needs, which installed tools were built with an older compiler, which repositories decode an image or a ZIP entry with no ceiling, which landing page is the odd one out — plus the shared landing design itself, a mutation runner that proves a test can fail, and a checks-waiter that refuses to call an empty check list a pass. |
| [`go-agentsync`](https://github.com/go-agentsync) | 1 | — | — | Coordination for sessions that share one machine: leases on repositories so two of them do not edit the same tree, a per-repository mailbox, and a memory index written back and read again, because an entry that reports success and then vanishes is indistinguishable from one never written. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
