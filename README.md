# LuminaSync Web

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Official **coming soon** landing page for [LuminaSync](https://github.com/LuminaSync). Static site deployed on [Vercel](https://vercel.com).

**Production:** [https://luminasync.vercel.app](https://luminasync.vercel.app)  
Custom domain `luminasync.vercel.com` can be added in the Vercel project settings.

## Stack

- Static HTML + CSS (no build step)
- Brand colors aligned with LuminaSync Core (`#0a0a0f`, `#00e5c0`, `#8b5cf6`)
- Brand images at repo root: `logo.png`, `logo-hero.png`, `favicon.ico`, `og-image.png`, `apple-touch-icon.png`, plus `logo-mark.svg` fallback

## Local preview

```powershell
cd LuminaSync-web
npx --yes serve . -p 3000
```

Open [http://localhost:3000](http://localhost:3000).

## Deploy on Vercel

1. Import the `LuminaSync-web` GitHub repository.
2. Framework preset: **Other** (no build command).
3. Output directory: `.` (repository root).
4. Production branch: `main`.
5. Optional: add domain `luminasync.vercel.com` → point DNS to Vercel.

`vercel.json`, `robots.txt`, and `sitemap.xml` are included.

## Ecosystem

| Repository | Role |
|------------|------|
| [LuminaSync-core](https://github.com/LuminaSync/LuminaSync-core) | Windows desktop app (GPL-3.0) |
| [LuminaSync-mobile](https://github.com/LuminaSync/LuminaSync-mobile) | Phone remote (GPL-3.0) |
| [LuminaSync-web](https://github.com/LuminaSync/LuminaSync-web) | This site (MIT) |

## Documentation

| File | Description |
|------|-------------|
| [docs/PROJECT.md](docs/PROJECT.md) | Site scope |
| [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) | SEO and future pages |

## License

MIT — see [LICENSE](LICENSE).
