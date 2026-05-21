# Web site architecture

## Role

Single-purpose **marketing and distribution** surface for LuminaSync. It does not run the display engine or mobile pairing logic.

## Deployment

| Item | Plan |
|------|------|
| Host | [Vercel](https://vercel.com) connected to `LuminaSync/LuminaSync-web` |
| Branch | `main` → production (maintainer-only repository) |
| Domain | Custom domain TBD (configure in Vercel + DNS) |

## Suggested stack (implementation)

- **Next.js** (static export or SSR) or **Astro** for content-heavy landing with minimal JS.
- Content in MDX or components under `src/` / `app/`.
- `public/` for `og-image.png`, favicon, platform icons.

## Page map

| Route | Purpose |
|-------|---------|
| `/` | Hero, value proposition, screenshot/GIF placeholder |
| `/#features` | Per-game profiles, tray app, mobile remote (planned) |
| `/#download` | Windows, Linux, Android, iOS buttons |
| `/#open-source` | Links to core, mobile, PoC (archived) repos |
| `/#support` | Buy Me a Coffee |

## SEO checklist

- [ ] `<title>` ≤ 60 chars, includes "LuminaSync" + primary keyword (e.g. game vibrance Windows)
- [ ] Meta description ~150–160 chars
- [ ] `link rel="canonical"`
- [ ] Open Graph: `og:title`, `og:description`, `og:image`, `og:url`
- [ ] Twitter card `summary_large_image`
- [ ] JSON-LD `SoftwareApplication` when downloads are live
- [ ] `sitemap.xml` + `robots.txt`
- [ ] `hreflang` only if translations ship
- [ ] Lighthouse: LCP, CLS, accessible contrast

## Download links policy

- **Windows:** GitHub Release asset from LuminaSync-core when published.
- **Linux:** Release or docs link when supported; otherwise disabled CTA.
- **Android / iOS:** Store URLs or "Coming soon" until LuminaSync-mobile ships.

Never imply a build exists without a real URL.

## Third-party

- **Buy Me a Coffee:** external link, `rel="noopener noreferrer"`.
- **GitHub:** org `https://github.com/LuminaSync`.

## License boundary

This site is **MIT**. Do not bundle GPL core source; link to GitHub for source and license text.
