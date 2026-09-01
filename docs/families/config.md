# Configuration management

The Puppet and Ansible stacks, in Go, without a Ruby or Python runtime.

| Organisation | Repos | Site | Docs | What it holds |
| --- | --- | --- | --- | --- |
| [`go-puppet`](https://github.com/go-puppet) | 1 | [site](https://go-puppet.github.io/) | [docs](https://go-puppet.github.io/docs/) | The Puppet language and its catalogue compiler. |
| [`go-pcore`](https://github.com/go-pcore) | 1 | [site](https://go-pcore.github.io/) | [docs](https://go-pcore.github.io/docs/) | Puppet's Pcore type system: type calculus, parser, value model, assignability lattice. |
| [`go-puppetdb`](https://github.com/go-puppetdb) | 1 | [site](https://go-puppetdb.github.io/) | [docs](https://go-puppetdb.github.io/docs/) | PuppetDB. |
| [`go-puppet-bolt`](https://github.com/go-puppet-bolt) | 1 | [site](https://go-puppet-bolt.github.io/) | [docs](https://go-puppet-bolt.github.io/docs/) | Bolt — task and plan orchestration over SSH and WinRM. |
| [`go-facter`](https://github.com/go-facter) | 1 | [site](https://go-facter.github.io/) | [docs](https://go-facter.github.io/docs/) | Fact collection. |
| [`go-hiera`](https://github.com/go-hiera) | 1 | [site](https://go-hiera.github.io/) | [docs](https://go-hiera.github.io/docs/) | Hierarchical data lookup. |
| [`go-eyaml`](https://github.com/go-eyaml) | 1 | [site](https://go-eyaml.github.io/) | [docs](https://go-eyaml.github.io/docs/) | eyaml — encrypted values inside Hiera data. |
| [`go-hocon`](https://github.com/go-hocon) | 1 | [site](https://go-hocon.github.io/) | [docs](https://go-hocon.github.io/docs/) | HOCON configuration. |
| [`go-augeas`](https://github.com/go-augeas) | 1 | [site](https://go-augeas.github.io/) | [docs](https://go-augeas.github.io/docs/) | The Augeas engine: a config tree, path expressions and lenses. |
| [`go-ansible`](https://github.com/go-ansible) | 10 | [site](https://go-ansible.github.io/) | [docs](https://go-ansible.github.io/docs/) | Ansible: inventory, variable precedence, Jinja2-compatible templating, connection and become plugins, the module protocol, and the playbook engine. |
| [`go-remoteexec`](https://github.com/go-remoteexec) | 1 | — | — | The layer both orchestrators run commands through: local, SSH and WinRM connections with sudo, su and doas escalation. |

Counts are public repositories that hold code; brand, docs and landing
repositories are excluded.
