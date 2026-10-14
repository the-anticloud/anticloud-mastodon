# MASTODON

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-social_media-lightgrey)

> Anticloud-hardened packaging of the upstream project `MASTODON` in category **SOCIAL MEDIA**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SOCIAL MEDIA · **Upstream:** https://github.com/mastodon/mastodon · **Upstream pin:** `336a62d850a28f6f066a26b83506ed70f0f4b906` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

> [!NOTE]
> Want to learn more about Mastodon?
> Click below to find out more in a video.

<p align="center">
  <a style="text-decoration:none" href="https://www.youtube.com/watch?v=IPSbNdBmWKE">
    <img alt="Mastodon hero image" src="./docs/hero-nodes.gif" />
  </a>
</p>

<p align="center">
  <a style="text-decoration:none" href="https://github.com/mastodon/mastodon/releases">
    <img src="https://img.shields.io/github/release/mastodon/mastodon.svg" alt="Release" /></a>
  <a style="text-decoration:none" href="https://github.com/mastodon/mastodon/actions/workflows/test-ruby.yml">
    <img src="https://github.com/mastodon/mastodon/actions/workflows/test-ruby.yml/badge.svg" alt="Ruby Testing" /></a>
  <a style="text-decoration:none" href="https://crowdin.com/project/mastodon">
    <img src="https://d322cqt584bo4o.cloudfront.net/mastodon/localized.svg" alt="Crowdin" /></a>
</p>

Mastodon is a **free, open-source social network server** based on [ActivityPub](https://www.w3.org/TR/activitypub/) where users can follow friends and discover new ones. On Mastodon, users can publish anything they want: links, pictures, text, and video. All Mastodon servers are interoperable as a federated network (users on one server can seamlessly communicate with users from another one, including non-Mastodon software that implements ActivityPub!)

## Navigation

- [Project homepage 🐘](https://joinmastodon.org)
- [Donate to support development 🎁](https://joinmastodon.org/sponsors#donate)
  - [View sponsors](https://joinmastodon.org/sponsors)
- [Blog 📰](https://blog.joinmastodon.org)
- [Documentation 📚](https://docs.joinmastodon.org)
- [Official container image 🚢](https://github.com/mastodon/mastodon/pkgs/container/mastodon)

## Features

<img src="./app/javascript/images/elephant_ui_working.svg?raw=true" align="right" width="30%" />

**Part of the Fediverse. Based on open standards, with no vendor lock-in.** - the network goes beyond just Mastodon; anything that implements ActivityPub is part of a broader social network known as [the Fediverse](https://jointhefediverse.net/). You can follow and interact with users on other servers (including those running different software), and they can follow you back.

**Real-time, chronological timeline updates** - updates of people you're following appear in real-time in the UI.

**Media attachments** - upload and view images and videos attached to the updates. Videos with no audio track are treated like animated GIFs; normal videos loop continuously.

**Safety and moderation tools** - Mastodon includes private posts, locked accounts, phrase filtering, muting, blocking, and many other features, along with a reporting and moderation system.

**OAuth2 and a straightforward REST API** - Mastodon acts as an OAuth2 provider, and third party apps can use the REST and Streaming APIs. This results in a [rich app ecosystem](https://joinmastodon.org/apps) with a variety of choices!

## Deployment

### Tech stack

- [Ruby on Rails](https://github.com/rails/rails) powers the REST API and other web pages.
- [PostgreSQL](https://www.postgresql.org/) is the main database.
- [Redis](https://redis.io/) and [Sidekiq](https://sidekiq.org/) are used for caching and queueing.
- [Node.js](https://nodejs.org/) powers the streaming API.
- [React.js](https://reactjs.org/) and [Redux](https://redux.js.org/) are used for the dynamic parts of the interface.
- [BrowserStack](https://www.browserstack.com/) supports testing on real devices and browsers. (This project is tested with BrowserStack)
- [Chromatic](https://www.chromatic.com/) provides visual regression testing. (This project is tested with Chromatic)

### Requirements

- **Ruby** 3.3+
- **PostgreSQL** 14+
- **Redis** 7.0+
- **Node.js** 22+
- **FFmpeg** 5.1+

This project includes deployment configurations for **Docker and docker-compose**, as well as for other environments like Heroku and Scalingo. For Helm charts, reference the [mastodon/chart project](https://github.com/mastodon/chart). A [**standalone** installation guide](https://docs.joinmastodon.org/admin/install/) is available in the main documentation.

## Contributing

Mastodon is **free, open-source software** licensed under **AGPLv3**. We welcome contributions and help from anyone who wants to improve the project.

You should read the overall [CONTRIBUTING](https://github.com/mastodon/.github/blob/main/CONTRIBUTING.md) guide, which covers our development processes.

You should also read and understand the [CODE OF CONDUCT](https://github.com/mastodon/.github/blob/main/CODE_OF_CONDUCT.md) that enables us to maintain a welcoming and inclusive community. Collaboration begins with mutual respect and understanding.

You can learn about setting up a development environment in the [DEVELOPMENT](docs/DEVELOPMENT.md) documentation.

If you would like to help with translations 🌐 you can do so on [Crowdin](https://crowdin.com/project/mastodon).

## LICENSE

Copyright (c) 2016-2026 Eugen Rochko (+ [`mastodon authors`](AUTHORS.md))

Licensed under GNU Affero General Public License as stated in the [LICENSE](LICENSE):

```text
Copyright (c) 2016-2026 Eugen Rochko & other Mastodon contributors

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU Affero General Public License as published by the Free
Software Foundation, either version 3 of the License, or (at your option) any
later version.

This program is distributed in the hope that it will be useful, but WITHOUT
ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License for more
details.

You should have received a copy of the GNU Affero General Public License along
with this program. If not, see https://www.gnu.org/licenses/
```

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Node.js / npm** (manifests: package.json, yarn.lock; scanned in UPSTREAM_CLONE)
- Top-level source layout: `app/`, `bin/`, `chart/`, `config/`, `db/`, `dist/`, `lib/`, `log/`, `public/`, `spec/`, `streaming/`, `vendor/`
- Snapshot size: **10001 files**, **303003 lines of code** (measured; see Benchmarks)
- Primary languages: `.svg` (4277), `.rb` (3277), `.yml` (553), `.tsx` (498), `.haml` (310), `.ts` (282)
- Upstream commit pinned for this packaging: `336a62d850a28f6f066a26b83506ed70f0f4b906`

---

## Installation

No installation section was found in the upstream readme, so the commands below are generated from the manifests detected in this project directory.

```sh
# from this project directory
npm install        # or: npm ci
npm run build      # if a build script is declared
```

Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

```sh
npm start          # declared start script, when present
npm run dev        # declared dev script, when present
```

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

<p align="center">
  <a style="text-decoration:none" href="https://www.youtube.com/watch?v=IPSbNdBmWKE">
    <img alt="Mastodon hero image" src="./docs/hero-nodes.gif" />
  </a>
</p>

<p align="center">
  <a style="text-decoration:none" href="https://github.com/mastodon/mastodon/releases">
    <img src="https://img.shields.io/github/release/mastodon/mastodon.svg" alt="Release" /></a>
  <a style="text-decoration:none" href="https://github.com/mastodon/mastodon/actions/workflows/test-ruby.yml">
    <img src="https://github.com/mastodon/mastodon/actions/workflows/test-ruby.yml/badge.svg" alt="Ruby Testing" /></a>
  <a style="text-decoration:none" href="https://crowdin.com/project/mastodon">
    <img src="https://d322cqt584bo4o.cloudfront.net/mastodon/localized.svg" alt="Crowdin" /></a>
</p>

Mastodon is a **free, open-source social network server** based on [ActivityPub](https://www.w3.org/TR/activitypub/) where users can follow friends and discover new ones. On Mastodon, users can publish anything they want: links, pictures, text, and video. All Mastodon servers are interoperable as a federated network (users on one server can seamlessly communicate with users from another one, including non-Mastodon software that implements ActivityPub!)

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Node.js / npm |
| Manifests detected | package.json, yarn.lock |
| Files in snapshot | 10001 |
| Lines of code | 303003 |
| Dependency references | 166 |
| Dependencies by ecosystem | npm: 166 |
| Upstream license | AGPL-3.0 |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| npm | @csstools/stylelint-formatter-github | 2.0.0 | package.json |
| npm | @dnd-kit/core | 6.3.1 | package.json |
| npm | @dnd-kit/modifiers | 9.0.0 | package.json |
| npm | @dnd-kit/sortable | 10.0.0 | package.json |
| npm | @dnd-kit/utilities | 3.2.2 | package.json |
| npm | @floating-ui/react-dom | 2.1.9 | package.json |
| npm | @formatjs/intl-pluralrules | 6.3.15 | package.json |
| npm | @formatjs/unplugin | 1.2.12 | package.json |
| npm | @gamestdio/websocket | 0.3.2 | package.json |
| npm | @github/webauthn-json | 2.1.1 | package.json |
| npm | @optimize-lodash/rollup-plugin | 6.0.0 | package.json |
| npm | @phosphor-icons/react | 2.1.10 | package.json |
| npm | @react-aria/utils | ^3.34.1 | package.json |
| npm | @react-spring/web | 10.1.2 | package.json |
| npm | @reduxjs/toolkit | 2.12.0 | package.json |
| ... | (151 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `.env.development`
- `.env.production.sample`
- `.env.test`
- `.env.vagrant`
- `Dockerfile`
- `config`
- `docker-compose.yml`
- `package.json`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contributing

Thank you for considering contributing to Mastodon 🐘

You can contribute in the following ways:

- Finding and reporting bugs
- Translating the Mastodon interface into various languages
- Contributing code to Mastodon by fixing bugs or implementing features
- Improving the documentation

Please review the org-level [contribution guidelines] for high-level acceptance
criteria guidance and the [DEVELOPMENT] guide for environment-specific details.
You should also read the project's [AI Contribution Policy] to understand how we approach
AI-assisted contributions.

## API Changes and Additions

Any changes or additions made to the API should have an accompanying pull
request on our [documentation project].

## Bug Reports

Bug reports and feature suggestions must use descriptive and concise titles and
be submitted to [GitHub Issues]. Please use the search function to make sure
there are not duplicate bug reports or feature requests.

## Security Issues

If you believe you have identified a security issue in Mastodon or our own apps,
check [SECURITY].

## Translations

Translations are community contributed via [Crowdin]. They are periodically
reviewed and merged into the codebase.

[![Crowdin](https://d322cqt584bo4o.cloudfront.net/mastodon/localized.svg)](https://crowdin.com/project/mastodon)

## Pull Requests

### Size and Scope

Our time is limited and PRs making large, unsolicited changes are unlikely to
get a response. Changes which link to an existing confirmed issue, or which come
from a "help wanted" issue or other request, are more likely to be reviewed.

The smaller and more narrowly focused the changes in a PR are, the easier they
are to review and potentially merge. If the change only makes sense in some
larger context of future ongoing work, note that in the description, but still
aim to keep each distinct PR to a "smallest viable change" chunk of work.

### Description of Changes

Unless the Pull Request is about refactoring code, updating dependencies or
other internal tasks, assume that the audience are not developers, but a
Mastodon user or server admin, and try to describe it from their perspective.

The final commit in the main branch will carry the title from the PR. The main
branch is then fed into the changelog and ultimately into release notes. We try
to follow the [keepachangelog] spec, and while that does not prescribe how
exactly the entries ought to be named, starting titles using one of the verbs
"Add", "Change", "D

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: AGPL-3.0** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
                    GNU AFFERO GENERAL PUBLIC LICENSE
                       Version 3, 19 November 2007

 Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
 Everyone is permitted to copy and distribute verbatim copies
 of this license document, but changing it is not allowed.

                            Preamble

  The GNU Affero General Public License is a free, copyleft license for
software and other kinds of works, specifically designed to ensure
cooperation with the community in the case of network server software.

  The licenses for most software and other practical works are designed
to take away your freedom to share and change the works.  By contrast,
our General Public Licenses are intended to guarantee your freedom to
share and change all versions of a program--to make sure it remains free
software for all its users.

  When we speak of free software, we are referring to freedom, not
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original AGPL-3.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `AGPL-3.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `MASTODON` (category: SOCIAL MEDIA)
- **Upstream URL:** https://github.com/mastodon/mastodon
- **Pinned commit (SHA):** `336a62d850a28f6f066a26b83506ed70f0f4b906`
- **Branch:** main
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`60f0dafbec2152de3c6b5b623514d8fb96ab6165dc76dceb7bd820ddcbe18cd3`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

