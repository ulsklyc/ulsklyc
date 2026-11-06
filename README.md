# Ulaş Kalaycı

**Maintainer of [Yuvomi](https://github.com/ulsklyc/yuvomi), the self-hosted family planner. Teacher of computer science, maths and social sciences in Germany, working on AI literacy and digital sovereignty in education.**

I build software that a household can run, own and leave: its data stays on its own server, nothing tracks it, and nothing locks it in. Open standards, MIT license, no cloud account with anyone.

[yuvomi.cloud](https://yuvomi.cloud) · [LinkedIn](https://www.linkedin.com/in/ulas-kalayci) · [Sponsor](https://github.com/sponsors/ulsklyc)

## Yuvomi

Tasks, calendar, budget, meals, shopping, health and documents for a family, in one PWA on a home server or NAS.

<p>
<a href="https://github.com/ulsklyc/yuvomi/releases"><img src="https://img.shields.io/github/v/release/ulsklyc/yuvomi?style=flat-square&color=6C3AED&label=release" alt="Latest release"></a>
<a href="https://github.com/ulsklyc/yuvomi/stargazers"><img src="https://img.shields.io/github/stars/ulsklyc/yuvomi?style=flat-square&color=6C3AED&label=stars" alt="GitHub stars"></a>
<a href="https://github.com/ulsklyc/yuvomi/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-6C3AED?style=flat-square" alt="MIT license"></a>
</p>

<a href="https://github.com/ulsklyc/yuvomi">
<picture>
<source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ulsklyc/yuvomi/main/docs/screenshots/dashboard-dark-web.webp">
<img src="https://raw.githubusercontent.com/ulsklyc/yuvomi/main/docs/screenshots/dashboard-light-web.webp" alt="The Yuvomi overview: today's events, tasks and shopping for the whole family" width="640">
</picture>
</a>

- **In development since March 2026** with Node.js, Express, SQLite and plain JavaScript. 20 modules, translated into 27 languages, runs on amd64 and arm64 in 256 MB of RAM. I'm the main maintainer; more than 40 people have contributed so far.
- **Installs** from the app catalogs of [Umbrel](https://github.com/getumbrel/umbrel-apps/tree/master/yuvomi), [TrueNAS SCALE](https://github.com/truenas/apps/tree/master/ix-dev/community/yuvomi) and [Unraid](https://yuvomi.cloud/install.html#unraid), with the [Proxmox community script](https://community-scripts.org/scripts/yuvomi), as a [Home Assistant app](https://github.com/ulsklyc/yuvomi-home-assistant) (started by [olli-dot-dev](https://github.com/olli-dot-dev), now maintained here), as a [YunoHost package](https://github.com/ulsklyc/yuvomi_ynh) (not in the YunoHost catalog yet), or with Docker or Podman. Every release opens an update pull request for the Umbrel app store automatically.
- **Covered by** [Caschys Blog](https://stadt-bremerhaven.de/yuvomi-open-source-familienplaner-zum-selbsthosten-buendelt-aufgaben-kalender-und-haushalt/), [mobiFlip](https://www.mobiflip.de/yuvomi-open-source-familienplaner-fuer-den-eigenen-server/) and [LinuxLinks](https://www.linuxlinks.com/yuvomi-self-hosted-family-planner-household-organiser/); setup guides by [mariushosting](https://mariushosting.com/how-to-install-yuvomi-on-your-synology-nas/) and [deployn on YouTube](https://www.youtube.com/watch?v=A0gRmsUnMGA).
- **Others build on it:** a [community handbook](https://github.com/Kyrodan/yuvomi-docs) by Kyrodan.

## How I build

- **Few moving parts, on purpose.** No frontend framework, no bundler, no CDN; third-party code is vendored by hand with its license. Fewer dependencies to update, audit and trust, and less to break for a family that updates once a year.
- **Rules live in tests.** The hard constraints - no framework imports, no `innerHTML`, every UI string in every language, database migrations that only ever grow at the end - fail the build instead of relying on good intentions.
- **A fix counts when a test proves it.** Every bug fix comes with a test that fails against the code before the fix.
- **AI agents, openly.** Much of the code is drafted with AI coding agents, and two of them, Claude Code and Codex, review pull requests independently of each other. I set the direction, the constraints and the tests they have to pass, and I answer for what ships. [How Yuvomi uses AI](https://github.com/ulsklyc/yuvomi/blob/main/CONTRIBUTING.md#ai-assistance)

## Teaching and research

I teach computer science, mathematics and social sciences at a comprehensive school in Dortmund. To me, AI literacy is computer science education: if you don't understand how models, data and infrastructure fit together, you learn to operate tools, not to think for yourself. At school I rebuilt the lower-secondary computer science curriculum, headed the department and designed in-house teacher training on large language models.

Yuvomi is where I put that into practice: AI agents draft much of the code, a human sets the constraints and answers for what ships, and the data stays with the people who create it.

**Research interests:** AI literacy and computer science education · digital sovereignty in educational institutions · teacher education on AI

Teaching also shapes how I write documentation, error messages and issue replies: for the person who has to understand them, not for the one who already does.

## Get in touch

- **Questions about Yuvomi:** [Discussions](https://github.com/ulsklyc/yuvomi/discussions)
- **Press, talks, research collaboration:** [info@yuvomi.cloud](mailto:info@yuvomi.cloud) or [LinkedIn](https://www.linkedin.com/in/ulas-kalayci)
- **Support the work:** [GitHub Sponsors](https://github.com/sponsors/ulsklyc)
