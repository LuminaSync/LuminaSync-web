# LuminaSync Web

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Official **landing page** and distribution hub for the [LuminaSync](https://github.com/LuminaSync) project. Built for [Vercel](https://vercel.com) with a strong **SEO** focus so users can find per-game display tuning for Windows (and upcoming mobile remote control) from search and social previews.

> **Status:** Documentation and site architecture defined; application scaffold (Next.js or Astro) to be added in a follow-up commit.

## Goals

- Explain what LuminaSync does in one screen: automatic color profiles when a game `.exe` is in focus.
- **Download** entry points for:
  - Windows
  - Linux (when a build is published)
  - Android and iOS (when the mobile app is published)
- **Open source** links to GitHub repositories.
- **Support** link (Buy Me a Coffee or equivalent).
- Fast, accessible layout; metadata and Open Graph tuned for discoverability.

## Ecosystem

| Repository | Role |
|------------|------|
| [LuminaSync-core](https://github.com/LuminaSync/LuminaSync-core) | Windows desktop app (GPL-3.0) |
| [LuminaSync-mobile](https://github.com/LuminaSync/LuminaSync-mobile) | Phone remote (GPL-3.0) |
| [LuminaSync-PoC](https://github.com/LuminaSync/LuminaSync-PoC) | Archived technical validation |
| [LuminaSync-web](https://github.com/LuminaSync/LuminaSync-web) | This site (MIT) |

## Documentation

| File | Description |
|------|-------------|
| [docs/PROJECT.md](docs/PROJECT.md) | Site scope and maintenance |
| [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) | Vercel deployment, page map, SEO checklist |

## Maintenance

This repository is **maintainer-only** (personal site). Feature work and community contributions belong in [LuminaSync-core](https://github.com/LuminaSync/LuminaSync-core) and [LuminaSync-mobile](https://github.com/LuminaSync/LuminaSync-mobile).

## Planned deployment

1. Connect this repository to Vercel.
2. Production branch: `main`.
3. Add custom domain when ready (DNS + Vercel project settings).

## Local development

Commands will be documented here after the framework is chosen (e.g. `pnpm dev` for Next.js).

## SEO targets (implementation)

- Unique title and meta description on the home page.
- Open Graph and Twitter card images under `public/`.
- `sitemap.xml` and `robots.txt`.
- Semantic headings and Core Web Vitals–friendly assets.

Details: [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md).

## License

MIT — see [LICENSE](LICENSE). LuminaSync Core and Mobile are GPL-3.0; this site links to them but does not embed their source.
