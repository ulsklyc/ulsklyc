# Ulaş Kalayci

**Maintainer of [Yuvomi](https://github.com/ulsklyc/yuvomi), the self-hosted family planner. Computer science and math teacher in Germany.**

I build software that a household can run, own and leave: its data stays on its own server, nothing tracks it, and nothing locks it in. Open standards, MIT license, no cloud account with anyone.

[yuvomi.cloud](https://yuvomi.cloud) · [LinkedIn](https://www.linkedin.com/in/ulas-kalayci-717087240) · [Sponsor](https://github.com/sponsors/ulsklyc)

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

- **In development since March 2026** with Node.js, Express, SQLite and plain JavaScript. Translated into 27 languages, runs on amd64 and arm64 in 256 MB of RAM.
- **In the app stores** of [Umbrel](https://github.com/getumbrel/umbrel-apps/tree/master/yuvomi), [TrueNAS](https://github.com/truenas/apps/tree/master/ix-dev/community/yuvomi) and Unraid, and as a [Proxmox community script](https://community-scripts.org/scripts/yuvomi). I bring the Umbrel package up to date with every release.
- **Covered by** [Caschys Blog](https://stadt-bremerhaven.de/yuvomi-open-source-familienplaner-zum-selbsthosten-buendelt-aufgaben-kalender-und-haushalt/), [deployn on YouTube](https://www.youtube.com/watch?v=A0gRmsUnMGA), [mariushosting](https://mariushosting.com/how-to-install-yuvomi-on-your-synology-nas/) and [Self-Host Weekly](https://selfh.st/weekly/2026-06-19/).
- **Others build on it:** a [Home Assistant add-on](https://github.com/olli-dot-dev/yuvomi-home-assistant) and a [community handbook](https://github.com/Kyrodan/yuvomi-docs).

## How I build

- **Few moving parts, on purpose.** No frontend framework, no bundler, no CDN; third-party code is vendored by hand with its license. Fewer dependencies to update, audit and trust, and less to break for a family that updates once a year.
- **Rules live in tests.** The hard constraints - no framework imports, no `innerHTML`, every UI string in every language, database migrations that only ever grow at the end - fail the build instead of relying on good intentions.
- **A fix counts when a test proves it.** Every bug fix comes with a test that fails against the code before the fix.
- **AI agents, openly.** Much of the code is drafted with AI coding agents, and two of them review pull requests automatically. I set the direction, the constraints and the tests they have to pass, and I answer for what ships. [How Yuvomi uses AI](https://github.com/ulsklyc/yuvomi/blob/main/CONTRIBUTING.md#ai-assistance)

## Beyond the code

Teaching computer science shapes how I write documentation, error messages and issue replies: for the person who has to understand them, not for the one who already does.

## Get in touch

- **Questions about Yuvomi:** [Discussions](https://github.com/ulsklyc/yuvomi/discussions)
- **Press, talks, collaboration:** [info@yuvomi.cloud](mailto:info@yuvomi.cloud) or [LinkedIn](https://www.linkedin.com/in/ulas-kalayci-717087240)
- **Support the work:** [GitHub Sponsors](https://github.com/sponsors/ulsklyc)
