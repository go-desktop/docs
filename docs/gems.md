# Ruby gems — one organisation each

A Ruby virtual machine is only useful with a library around it, so each gem the
ecosystem needs is reimplemented in pure Go in its own `go-ruby-*` organisation:
the standard library, Rails and its dependencies, the testing stack, the Puppet
stack, database drivers, serialisation formats and template engines.

Every one of them is byte-compared against MRI where a byte comparison is
meaningful — a checksum, a `Marshal` payload, a formatted number. Where it is not
(a deflate stream, say, whose output is implementation-defined) the requirement is
interoperability in both directions instead.

Two things to know before reaching for one:

- **The gem organisation is the Ruby-facing wrapper, not always the engine.** Some
  are thin shells over an engine that lives in its own non-Ruby organisation — the
  regexp gem wraps [`go-regexp/engine`](https://github.com/go-regexp/engine), the
  sass gem wraps [`go-scss/scss`](https://github.com/go-scss/scss). If you are
  writing Go rather than Ruby, take the engine.
- **The repository inside is named after the gem**, not after the organisation:
  `go-ruby-activerecord/activerecord`.

| Gem | Organisation |
| --- | --- |
| `aasm` | [`go-ruby-aasm`](https://github.com/go-ruby-aasm) |
| `abbrev` | [`go-ruby-abbrev`](https://github.com/go-ruby-abbrev) |
| `acme` | [`go-ruby-acme`](https://github.com/go-ruby-acme) |
| `actioncable` | [`go-ruby-actioncable`](https://github.com/go-ruby-actioncable) |
| `actionmailer` | [`go-ruby-actionmailer`](https://github.com/go-ruby-actionmailer) |
| `actionpack` | [`go-ruby-actionpack`](https://github.com/go-ruby-actionpack) |
| `actionview` | [`go-ruby-actionview`](https://github.com/go-ruby-actionview) |
| `activejob` | [`go-ruby-activejob`](https://github.com/go-ruby-activejob) |
| `activeldap` | [`go-ruby-activeldap`](https://github.com/go-ruby-activeldap) |
| `activemodel` | [`go-ruby-activemodel`](https://github.com/go-ruby-activemodel) |
| `activerecord` | [`go-ruby-activerecord`](https://github.com/go-ruby-activerecord) |
| `activestorage` | [`go-ruby-activestorage`](https://github.com/go-ruby-activestorage) |
| `activesupport` | [`go-ruby-activesupport`](https://github.com/go-ruby-activesupport) |
| `addressable` | [`go-ruby-addressable`](https://github.com/go-ruby-addressable) |
| `age` | [`go-ruby-age`](https://github.com/go-ruby-age) |
| `arrow` | [`go-ruby-arrow`](https://github.com/go-ruby-arrow) |
| `async` | [`go-ruby-async`](https://github.com/go-ruby-async) |
| `augeas` | [`go-ruby-augeas`](https://github.com/go-ruby-augeas) |
| `base64` | [`go-ruby-base64`](https://github.com/go-ruby-base64) |
| `bbolt` | [`go-ruby-bbolt`](https://github.com/go-ruby-bbolt) |
| `bcrypt` | [`go-ruby-bcrypt`](https://github.com/go-ruby-bcrypt) |
| `benchmark` | [`go-ruby-benchmark`](https://github.com/go-ruby-benchmark) |
| `bigdecimal` | [`go-ruby-bigdecimal`](https://github.com/go-ruby-bigdecimal) |
| `bleve` | [`go-ruby-bleve`](https://github.com/go-ruby-bleve) |
| `builder` | [`go-ruby-builder`](https://github.com/go-ruby-builder) |
| `bundler` | [`go-ruby-bundler`](https://github.com/go-ruby-bundler) |
| `cancancan` | [`go-ruby-cancancan`](https://github.com/go-ruby-cancancan) |
| `capistrano` | [`go-ruby-capistrano`](https://github.com/go-ruby-capistrano) |
| `capybara` | [`go-ruby-capybara`](https://github.com/go-ruby-capybara) |
| `cgi` | [`go-ruby-cgi`](https://github.com/go-ruby-cgi) |
| `chronic` | [`go-ruby-chronic`](https://github.com/go-ruby-chronic) |
| `cmath` | [`go-ruby-cmath`](https://github.com/go-ruby-cmath) |
| `commonmark` | [`go-ruby-commonmark`](https://github.com/go-ruby-commonmark) |
| `complex` | [`go-ruby-complex`](https://github.com/go-ruby-complex) |
| `concurrent-ruby` | [`go-ruby-concurrent-ruby`](https://github.com/go-ruby-concurrent-ruby) |
| `confd` | [`go-ruby-confd`](https://github.com/go-ruby-confd) |
| `connection-pool` | [`go-ruby-connection-pool`](https://github.com/go-ruby-connection-pool) |
| `csv` | [`go-ruby-csv`](https://github.com/go-ruby-csv) |
| `date` | [`go-ruby-date`](https://github.com/go-ruby-date) |
| `deep-merge` | [`go-ruby-deep-merge`](https://github.com/go-ruby-deep-merge) |
| `devise` | [`go-ruby-devise`](https://github.com/go-ruby-devise) |
| `did-you-mean` | [`go-ruby-did-you-mean`](https://github.com/go-ruby-did-you-mean) |
| `digest` | [`go-ruby-digest`](https://github.com/go-ruby-digest) |
| `dotenv` | [`go-ruby-dotenv`](https://github.com/go-ruby-dotenv) |
| `dry-struct` | [`go-ruby-dry-struct`](https://github.com/go-ruby-dry-struct) |
| `dry-types` | [`go-ruby-dry-types`](https://github.com/go-ruby-dry-types) |
| `dry-validation` | [`go-ruby-dry-validation`](https://github.com/go-ruby-dry-validation) |
| `erasure` | [`go-ruby-erasure`](https://github.com/go-ruby-erasure) |
| `erb` | [`go-ruby-erb`](https://github.com/go-ruby-erb) |
| `erubi` | [`go-ruby-erubi`](https://github.com/go-ruby-erubi) |
| `etcd` | [`go-ruby-etcd`](https://github.com/go-ruby-etcd) |
| `excon` | [`go-ruby-excon`](https://github.com/go-ruby-excon) |
| `facter` | [`go-ruby-facter`](https://github.com/go-ruby-facter) |
| `factory-bot` | [`go-ruby-factory-bot`](https://github.com/go-ruby-factory-bot) |
| `faker` | [`go-ruby-faker`](https://github.com/go-ruby-faker) |
| `faraday` | [`go-ruby-faraday`](https://github.com/go-ruby-faraday) |
| `fast-gettext` | [`go-ruby-fast-gettext`](https://github.com/go-ruby-fast-gettext) |
| `fast-gettext-locale` | [`go-ruby-fast-gettext-locale`](https://github.com/go-ruby-fast-gettext-locale) |
| `find` | [`go-ruby-find`](https://github.com/go-ruby-find) |
| `format` | [`go-ruby-format`](https://github.com/go-ruby-format) |
| `friendly-id` | [`go-ruby-friendly-id`](https://github.com/go-ruby-friendly-id) |
| `fsctl` | [`go-ruby-fsctl`](https://github.com/go-ruby-fsctl) |
| `getoptlong` | [`go-ruby-getoptlong`](https://github.com/go-ruby-getoptlong) |
| `grape` | [`go-ruby-grape`](https://github.com/go-ruby-grape) |
| `graphql` | [`go-ruby-graphql`](https://github.com/go-ruby-graphql) |
| `grpc` | [`go-ruby-grpc`](https://github.com/go-ruby-grpc) |
| `haml` | [`go-ruby-haml`](https://github.com/go-ruby-haml) |
| `hanami` | [`go-ruby-hanami`](https://github.com/go-ruby-hanami) |
| `hcl2` | [`go-ruby-hcl2`](https://github.com/go-ruby-hcl2) |
| `hiera` | [`go-ruby-hiera`](https://github.com/go-ruby-hiera) |
| `hiera-eyaml` | [`go-ruby-hiera-eyaml`](https://github.com/go-ruby-hiera-eyaml) |
| `hocon` | [`go-ruby-hocon`](https://github.com/go-ruby-hocon) |
| `http` | [`go-ruby-http`](https://github.com/go-ruby-http) |
| `httparty` | [`go-ruby-httparty`](https://github.com/go-ruby-httparty) |
| `i18n` | [`go-ruby-i18n`](https://github.com/go-ruby-i18n) |
| `images` | [`go-ruby-images`](https://github.com/go-ruby-images) |
| `ipaddr` | [`go-ruby-ipaddr`](https://github.com/go-ruby-ipaddr) |
| `irb` | [`go-ruby-irb`](https://github.com/go-ruby-irb) |
| `jbuilder` | [`go-ruby-jbuilder`](https://github.com/go-ruby-jbuilder) |
| `jekyll` | [`go-ruby-jekyll`](https://github.com/go-ruby-jekyll) |
| `json` | [`go-ruby-json`](https://github.com/go-ruby-json) |
| `jwt` | [`go-ruby-jwt`](https://github.com/go-ruby-jwt) |
| `kafka` | [`go-ruby-kafka`](https://github.com/go-ruby-kafka) |
| `kaminari` | [`go-ruby-kaminari`](https://github.com/go-ruby-kaminari) |
| `kramdown` | [`go-ruby-kramdown`](https://github.com/go-ruby-kramdown) |
| `ldap` | [`go-ruby-ldap`](https://github.com/go-ruby-ldap) |
| `liquid` | [`go-ruby-liquid`](https://github.com/go-ruby-liquid) |
| `logger` | [`go-ruby-logger`](https://github.com/go-ruby-logger) |
| `mail` | [`go-ruby-mail`](https://github.com/go-ruby-mail) |
| `marshal` | [`go-ruby-marshal`](https://github.com/go-ruby-marshal) |
| `matrix` | [`go-ruby-matrix`](https://github.com/go-ruby-matrix) |
| `mime-types` | [`go-ruby-mime-types`](https://github.com/go-ruby-mime-types) |
| `minitest` | [`go-ruby-minitest`](https://github.com/go-ruby-minitest) |
| `money` | [`go-ruby-money`](https://github.com/go-ruby-money) |
| `mongodb` | [`go-ruby-mongodb`](https://github.com/go-ruby-mongodb) |
| `msgpack` | [`go-ruby-msgpack`](https://github.com/go-ruby-msgpack) |
| `multi-json` | [`go-ruby-multi-json`](https://github.com/go-ruby-multi-json) |
| `mustache` | [`go-ruby-mustache`](https://github.com/go-ruby-mustache) |
| `mysql` | [`go-ruby-mysql`](https://github.com/go-ruby-mysql) |
| `nats` | [`go-ruby-nats`](https://github.com/go-ruby-nats) |
| `net-ftp` | [`go-ruby-net-ftp`](https://github.com/go-ruby-net-ftp) |
| `net-http` | [`go-ruby-net-http`](https://github.com/go-ruby-net-http) |
| `net-imap` | [`go-ruby-net-imap`](https://github.com/go-ruby-net-imap) |
| `net-pop` | [`go-ruby-net-pop`](https://github.com/go-ruby-net-pop) |
| `net-s3` | [`go-ruby-net-s3`](https://github.com/go-ruby-net-s3) |
| `net-sftp` | [`go-ruby-net-sftp`](https://github.com/go-ruby-net-sftp) |
| `net-smtp` | [`go-ruby-net-smtp`](https://github.com/go-ruby-net-smtp) |
| `nokogiri` | [`go-ruby-nokogiri`](https://github.com/go-ruby-nokogiri) |
| `oauth2` | [`go-ruby-oauth2`](https://github.com/go-ruby-oauth2) |
| `observer` | [`go-ruby-observer`](https://github.com/go-ruby-observer) |
| `oidc` | [`go-ruby-oidc`](https://github.com/go-ruby-oidc) |
| `omniauth` | [`go-ruby-omniauth`](https://github.com/go-ruby-omniauth) |
| `openbao` | [`go-ruby-openbao`](https://github.com/go-ruby-openbao) |
| `openssl` | [`go-ruby-openssl`](https://github.com/go-ruby-openssl) |
| `openstack` | [`go-ruby-openstack`](https://github.com/go-ruby-openstack) |
| `opentelemetry` | [`go-ruby-opentelemetry`](https://github.com/go-ruby-opentelemetry) |
| `opentype` | [`go-ruby-opentype`](https://github.com/go-ruby-opentype) |
| `optparse` | [`go-ruby-optparse`](https://github.com/go-ruby-optparse) |
| `ostruct` | [`go-ruby-ostruct`](https://github.com/go-ruby-ostruct) |
| `pagy` | [`go-ruby-pagy`](https://github.com/go-ruby-pagy) |
| `paper-trail` | [`go-ruby-paper-trail`](https://github.com/go-ruby-paper-trail) |
| `parquet` | [`go-ruby-parquet`](https://github.com/go-ruby-parquet) |
| `parser` | [`go-ruby-parser`](https://github.com/go-ruby-parser) |
| `pathname` | [`go-ruby-pathname`](https://github.com/go-ruby-pathname) |
| `pg` | [`go-ruby-pg`](https://github.com/go-ruby-pg) |
| `prawn` | [`go-ruby-prawn`](https://github.com/go-ruby-prawn) |
| `prettyprint` | [`go-ruby-prettyprint`](https://github.com/go-ruby-prettyprint) |
| `prime` | [`go-ruby-prime`](https://github.com/go-ruby-prime) |
| `protobuf` | [`go-ruby-protobuf`](https://github.com/go-ruby-protobuf) |
| `pstore` | [`go-ruby-pstore`](https://github.com/go-ruby-pstore) |
| `public-suffix` | [`go-ruby-public-suffix`](https://github.com/go-ruby-public-suffix) |
| `puma` | [`go-ruby-puma`](https://github.com/go-ruby-puma) |
| `pundit` | [`go-ruby-pundit`](https://github.com/go-ruby-pundit) |
| `puppet` | [`go-ruby-puppet`](https://github.com/go-ruby-puppet) |
| `puppet-resource-api` | [`go-ruby-puppet-resource-api`](https://github.com/go-ruby-puppet-resource-api) |
| `racc` | [`go-ruby-racc`](https://github.com/go-ruby-racc) |
| `rack` | [`go-ruby-rack`](https://github.com/go-ruby-rack) |
| `rails` | [`go-ruby-rails`](https://github.com/go-ruby-rails) |
| `railties` | [`go-ruby-railties`](https://github.com/go-ruby-railties) |
| `rake` | [`go-ruby-rake`](https://github.com/go-ruby-rake) |
| `ransack` | [`go-ruby-ransack`](https://github.com/go-ruby-ransack) |
| `rational` | [`go-ruby-rational`](https://github.com/go-ruby-rational) |
| `rdoc` | [`go-ruby-rdoc`](https://github.com/go-ruby-rdoc) |
| `reddit` | [`go-ruby-reddit`](https://github.com/go-ruby-reddit) |
| `redis` | [`go-ruby-redis`](https://github.com/go-ruby-redis) |
| `regexp` | [`go-ruby-regexp`](https://github.com/go-ruby-regexp) |
| `reline` | [`go-ruby-reline`](https://github.com/go-ruby-reline) |
| `resolv` | [`go-ruby-resolv`](https://github.com/go-ruby-resolv) |
| `resque` | [`go-ruby-resque`](https://github.com/go-ruby-resque) |
| `rexml` | [`go-ruby-rexml`](https://github.com/go-ruby-rexml) |
| `roda` | [`go-ruby-roda`](https://github.com/go-ruby-roda) |
| `rolify` | [`go-ruby-rolify`](https://github.com/go-ruby-rolify) |
| `rouge` | [`go-ruby-rouge`](https://github.com/go-ruby-rouge) |
| `rqrcode` | [`go-ruby-rqrcode`](https://github.com/go-ruby-rqrcode) |
| `rspec` | [`go-ruby-rspec`](https://github.com/go-ruby-rspec) |
| `rss` | [`go-ruby-rss`](https://github.com/go-ruby-rss) |
| `rubocop` | [`go-ruby-rubocop`](https://github.com/go-ruby-rubocop) |
| `rubygems` | [`go-ruby-rubygems`](https://github.com/go-ruby-rubygems) |
| `saml` | [`go-ruby-saml`](https://github.com/go-ruby-saml) |
| `sass` | [`go-ruby-sass`](https://github.com/go-ruby-sass) |
| `scanf` | [`go-ruby-scanf`](https://github.com/go-ruby-scanf) |
| `securerandom` | [`go-ruby-securerandom`](https://github.com/go-ruby-securerandom) |
| `semantic-puppet` | [`go-ruby-semantic-puppet`](https://github.com/go-ruby-semantic-puppet) |
| `sequel` | [`go-ruby-sequel`](https://github.com/go-ruby-sequel) |
| `set` | [`go-ruby-set`](https://github.com/go-ruby-set) |
| `shellwords` | [`go-ruby-shellwords`](https://github.com/go-ruby-shellwords) |
| `shrine` | [`go-ruby-shrine`](https://github.com/go-ruby-shrine) |
| `sidekiq` | [`go-ruby-sidekiq`](https://github.com/go-ruby-sidekiq) |
| `simplecov` | [`go-ruby-simplecov`](https://github.com/go-ruby-simplecov) |
| `sinatra` | [`go-ruby-sinatra`](https://github.com/go-ruby-sinatra) |
| `slim` | [`go-ruby-slim`](https://github.com/go-ruby-slim) |
| `sodium` | [`go-ruby-sodium`](https://github.com/go-ruby-sodium) |
| `sqlite3` | [`go-ruby-sqlite3`](https://github.com/go-ruby-sqlite3) |
| `stdlib` | [`go-ruby-stdlib`](https://github.com/go-ruby-stdlib) |
| `stringio` | [`go-ruby-stringio`](https://github.com/go-ruby-stringio) |
| `strscan` | [`go-ruby-strscan`](https://github.com/go-ruby-strscan) |
| `syslog` | [`go-ruby-syslog`](https://github.com/go-ruby-syslog) |
| `thor` | [`go-ruby-thor`](https://github.com/go-ruby-thor) |
| `time` | [`go-ruby-time`](https://github.com/go-ruby-time) |
| `timecop` | [`go-ruby-timecop`](https://github.com/go-ruby-timecop) |
| `toml` | [`go-ruby-toml`](https://github.com/go-ruby-toml) |
| `tsort` | [`go-ruby-tsort`](https://github.com/go-ruby-tsort) |
| `typhoeus` | [`go-ruby-typhoeus`](https://github.com/go-ruby-typhoeus) |
| `tzinfo` | [`go-ruby-tzinfo`](https://github.com/go-ruby-tzinfo) |
| `unicode-normalize` | [`go-ruby-unicode-normalize`](https://github.com/go-ruby-unicode-normalize) |
| `uri` | [`go-ruby-uri`](https://github.com/go-ruby-uri) |
| `vcr` | [`go-ruby-vcr`](https://github.com/go-ruby-vcr) |
| `warden` | [`go-ruby-warden`](https://github.com/go-ruby-warden) |
| `webauthn` | [`go-ruby-webauthn`](https://github.com/go-ruby-webauthn) |
| `webmock` | [`go-ruby-webmock`](https://github.com/go-ruby-webmock) |
| `webrick` | [`go-ruby-webrick`](https://github.com/go-ruby-webrick) |
| `xslt` | [`go-ruby-xslt`](https://github.com/go-ruby-xslt) |
| `yaml` | [`go-ruby-yaml`](https://github.com/go-ruby-yaml) |
| `zeitwerk` | [`go-ruby-zeitwerk`](https://github.com/go-ruby-zeitwerk) |
| `zlib` | [`go-ruby-zlib`](https://github.com/go-ruby-zlib) |

195 gem organisations, 195 public code repositories.
