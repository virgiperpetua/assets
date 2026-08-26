# Virginia Perpetua Assets

Binary brand assets — wordmark, VP mark, portrait, banners, Open Graph / LinkedIn art, and page screenshots from the Claude Design portfolio.

Token values live in [`tokens`](https://gitlab.com/virginia-perpetua/design-system/tokens). Marketing pages live in [`marketing`](https://gitlab.com/virginia-perpetua/design-system/marketing). Brand rules: [BRAND.md](./BRAND.md). Design export specs: [docs/design-export/](./docs/design-export/).

## At a glance

| Asset | Preview | Default download |
| ----- | ------- | ---------------- |
| **Dark mark** (512) | [<img src="./dist/logo/mark/dark/bg-none/512.png" alt="Dark mark" width="96" height="96">](./dist/logo/mark/dark/bg-none/512.png) | [512.png](./dist/logo/mark/dark/bg-none/512.png) |
| **Light mark** (512) | [<img src="./dist/logo/mark/light/bg-none/512.png" alt="Light mark" width="96" height="96">](./dist/logo/mark/light/bg-none/512.png) | [512.png](./dist/logo/mark/light/bg-none/512.png) |
| **Wordmark dark** | [<img src="./dist/logo/wordmark/dark/bg-none/640.png" alt="Wordmark dark" width="240">](./dist/logo/wordmark/dark/bg-none/640.png) | [640.png](./dist/logo/wordmark/dark/bg-none/640.png) |
| **Portrait** | [<img src="./dist/photo/virginia-photo.png" alt="Portrait" width="96" height="96">](./dist/photo/virginia-photo.png) | [virginia-photo.png](./dist/photo/virginia-photo.png) |
| **LinkedIn / OG banner** | [<img src="./dist/og-image/linkedin-banner.png" alt="OG banner" width="240">](./dist/og-image/linkedin-banner.png) | [linkedin-banner.png](./dist/og-image/linkedin-banner.png) |

## Layout

```text
src/logo/{wordmark,mark}/{dark|light}/…   # masters + PNG sizes
src/photo/                                 # portrait
src/og-image/                              # social share art
src/banners/                               # campaign / LinkedIn composites
src/screenshots/pages/                     # full-page design captures
docs/design-export/                        # Markdown specs paired with screenshots
dist/                                      # publish tree (mirrors src binaries)
portfolio/                                 # Claude Design source (*.dc.html)
```

## CDN-style paths

When served from Pages (or a CDN), treat `dist/` as the site root:

```text
/logo/mark/{dark|light}/bg-none/{32|256|512}.png
/logo/wordmark/{dark|light}/bg-none/{640|1280}.png
/photo/virginia-photo.png
/og-image/linkedin-banner.png
/screenshots/pages/{home|about|projects|resume|contact|linkedin-banner|brand-system-spec}.png
```
