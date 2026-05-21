# Project overview

Marketing and distribution site for the LuminaSync ecosystem: landing page, platform downloads, links to GitHub, and support (e.g. Buy Me a Coffee). Hosted on **Vercel**.

## Ecosystem

| Repo | Role | License |
|------|------|---------|
| [LuminaSync-core](https://github.com/LuminaSync/LuminaSync-core) | Windows desktop | GPL-3.0 |
| [LuminaSync-mobile](https://github.com/LuminaSync/LuminaSync-mobile) | Android / iOS remote | GPL-3.0 |
| [LuminaSync-PoC](https://github.com/LuminaSync/LuminaSync-PoC) | Archived PoC | — |
| [LuminaSync-web](https://github.com/LuminaSync/LuminaSync-web) | This site | MIT |

## Tech direction

- Static or SSR framework suited to Vercel (Next.js, Astro, or similar).
- **SEO first:** metadata, Open Graph, `sitemap.xml`, `robots.txt`, semantic headings, Core Web Vitals.
- English primary copy; structure ready for i18n later if needed.

## Content requirements

- Hero: per-game color profiles on Windows.
- Download CTAs: Windows, Linux, Android, iOS (honest “coming soon” until releases exist).
- Links: GitHub org/repos, core contributing guide, license badges.
- Support: Buy Me a Coffee (or equivalent).

## Maintenance

Maintainer-only repository. Code contributions belong in LuminaSync-core and LuminaSync-mobile.

## Out of scope

- Windows display APIs
- Mobile WebSocket server
- Bundling GPL core source (link to GitHub instead)

See [ARCHITECTURE.md](ARCHITECTURE.md) for deployment and SEO.
