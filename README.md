# neto4ka.github.io

[![Live site](https://img.shields.io/badge/live-neto4ka.github.io-b5e853?style=flat-square&labelColor=000000)](https://neto4ka.github.io/)[![License: GPL v3](https://img.shields.io/badge/license-GPLv3-blue?style=flat-square)](https://www.gnu.org/licenses/gpl-3.0)
[![Delta Chat](https://img.shields.io/badge/Delta_Chat-channel-317da8?style=flat-square)](https://deltachat.id/neto4ka)

Source of **[neto4ka.github.io](https://neto4ka.github.io/)** — a static site
built with Jekyll and hosted on GitHub Pages: terminal-style UI,
syntax-highlighted code blocks and an interactive network graph. Also contains
ASCII art, code poetry, Perl poetry. No frameworks, no build step.

## Contact

Public channel on **Delta Chat**. Scan the QR code to join, or open the link —
the page greets newcomers and opens the channel for app users.

<img src="assets/deltachat-qr.svg" width="200" alt="Delta Chat channel invite QR code: deltachat.id/neto4ka">

- **Channel:** [deltachat.id/neto4ka](https://deltachat.id/neto4ka)
- **GitHub:** [@Neto4ka](https://github.com/Neto4ka)

## Features

- **Jekyll + GitHub Pages** — push to `main`, the site rebuilds and deploys automatically.
- **Terminal-style UI** — monospace layout, CRT scanline effect and a neon palette
  driven by CSS custom properties; responsive down to small screens.
- **Syntax highlighting** — server-rendered code blocks via Jekyll / Rouge.
- **Interactive graph** — [vis-network](https://github.com/visjs/vis-network) 10.1.5:
  99 nodes / 98 edges, depth filtering (1–6), re-center and fullscreen controls.
- **Performance** — the graph library is lazy-loaded from a CDN only when the graph
  scrolls into view (`IntersectionObserver` + `requestIdleCallback`); the physics
  simulation pauses off-screen.
- **Accessible & responsive** — `prefers-reduced-motion` support, keyboard-focusable
  controls, `ResizeObserver`-based canvas resizing, Fullscreen API with a CSS fallback.
- **Zero dependencies** — vanilla HTML / CSS / JS, nothing to install or bundle.

## Repository structure

| Path | Description |
| --- | --- |
| [`_config.yml`](_config.yml) | Jekyll configuration (theme, title, description) |
| [`index.md`](index.md) | Main page: layout, content and styles |
| [`_includes/graph.html`](_includes/graph.html) | Network graph: markup, styles and JavaScript |
| [`assets/deltachat-qr.svg`](assets/deltachat-qr.svg) | Delta Chat channel invite QR code |
| [`LICENSE`](LICENSE) | GNU General Public License v3.0 |

## Getting started

```bash
gem install jekyll jekyll-theme-hacker
jekyll serve
# → http://localhost:4000
```

## Deployment

Every push to `main` triggers a GitHub Pages build. See the
[deployments](https://github.com/Neto4ka/neto4ka.github.io/deployments) for build history.

## Contributing

Issues and pull requests are welcome.

## License

Copyright (C) 2026 Neto4ka. Licensed under the
[GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0).
See [LICENSE](LICENSE).
