# The map itself

The one thing this organisation does hold: the tool that generates every page here.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-desktop`](https://github.com/go-desktop) | 1 | [site](https://go-desktop.github.io/) | [docs](https://go-desktop.github.io/docs/) | The generator. It reads the live GitHub organisation list and reconciles it against a curated classification, then writes the landing configuration, the family pages, the gem list and this profile. The reconciliation is the point: an organisation that holds code but is in no family fails the build, so the index cannot quietly omit something that exists. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
