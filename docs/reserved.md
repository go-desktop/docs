# Held, not yet built

These organisation names are reserved and empty. They are listed so the map has no
silent gaps: an empty organisation is not a shipped one, and a name that looks like
a capability is the easiest way to believe a capability exists.

| Organisation | Intended for |
| --- | --- |
| [`go-graphdrawing`](https://github.com/go-graphdrawing) | Graph-drawing algorithms — Sugiyama layering, force-directed placement, trees. Deliberately not started for TeX's sake: the measurement that settled it found pgf's `graphdrawing` used by 5 documents in a 10,025-talk corpus, the worst effort-to-impact ratio in the plan. It will begin when diagrams in an editor or a toolkit need it. |
| [`go-grub`](https://github.com/go-grub) | Superseded in practice by [`go-bootloaders/grub`](https://github.com/go-bootloaders/grub). |
| [`go-quake2`](https://github.com/go-quake2) | A Quake II engine, after [`go-quake1`](https://github.com/go-quake1). |
| [`go-quake3`](https://github.com/go-quake3) | A Quake III engine. |
| [`go-sicp`](https://github.com/go-sicp) | Reserved. |
| [`go-ruby-atproto`](https://github.com/go-ruby-atproto) · [`go-ruby-birdsite`](https://github.com/go-ruby-birdsite) · [`go-ruby-hackernews`](https://github.com/go-ruby-hackernews) · [`go-ruby-instagram`](https://github.com/go-ruby-instagram) · [`go-ruby-mastodon`](https://github.com/go-ruby-mastodon) · [`go-ruby-newsgroups`](https://github.com/go-ruby-newsgroups) · [`go-ruby-syndication`](https://github.com/go-ruby-syndication) · [`go-ruby-tiktok`](https://github.com/go-ruby-tiktok) | Ruby-facing wrappers for the social and feed clients that already exist in Go. |

## Not in this map

Two sibling stacks are deliberately **not** Go, and are not counted anywhere on
this site:

| Organisation | What it is |
| --- | --- |

Separately, a handful of organisations hold research-computing and OpenStack
operations work — images, Terraform modules, CI provisioners, JupyterHub
infrastructure — in shell, HCL, Groovy and Python. They are real and maintained;
they are simply not part of the Go library ecosystem this site maps.

## One retired organisation

`go-onigmo` was **deleted** in August 2026. It had briefly hosted what is now
[`go-ruby-regexp`](https://github.com/go-ruby-regexp), which left every plausible
name under it behaving as a retired redirect — a clone that looked like it worked
and silently pointed somewhere else. The engine lives at
[`go-regexp/engine`](https://github.com/go-regexp/engine).

The lesson generalises to anything in this map: resolve an organisation and
repository before depending on it, rather than assuming the name means what it
says.
