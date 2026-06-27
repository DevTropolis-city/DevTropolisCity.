# DEVTROPOLIS

**Turn any GitHub profile into a glowing 3D city.**

Enter a GitHub username → real public profile data is fetched → a unique isometric 3D skyline is built live in the browser, district by district, repo by repo.

[![Live Demo](https://img.shields.io/badge/Live_Demo-devtropolis-FF9E00?style=flat-square)](https://devtropolis-city.github.io/DevTropolisCity/)
[![Stars](https://img.shields.io/github/stars/DevTropolis-city/DevTropolisCity?style=flat-square&color=00B4D8)](https://github.com/DevTropolis-city/DevTropolisCity/stargazers)
[![License](https://img.shields.io/badge/license-MIT-00B4D8?style=flat-square)](https://github.com/DevTropolis-city/DevTropolisCity/blob/main/LICENSE)
[![Three.js](https://img.shields.io/badge/Three.js-black?style=flat-square&logo=three.js)](https://threejs.org)
[![No Build Step](https://img.shields.io/badge/build_step-none-success?style=flat-square)](#)

---

## What is DevTropolis?

**DevTropolis** is a single-page, single-file web app that reverse-engineers a GitHub profile into a city. Repos become buildings, languages become districts and lighting, stars and followers shape the skyline. No login, no backend, no build step — just a GitHub username and a browser with WebGL.

Inspired by the idea that a developer's public footprint deserves a skyline, not just a contribution graph.

---

## How it works

```
01 — Enter username   →   02 — Fetch GitHub data   →   03 — City is built

   "torvalds"              public REST API              live 3D skyline
```

1. **Enter a username** — or paste a `github.com/...` URL
2. **DevTropolis fetches** — profile, repos, languages, stars, followers via the public GitHub API
3. **The city renders** — districts, buildings, traffic, and lights generated live with Three.js

---

## Features

| Feature | Description |
|---|---|
| 🏙️ Procedural 3D city | Skyline generated live from real GitHub profile + repo data |
| 🌆 Language districts | Dominant languages drive district placement and building color/lighting |
| 🏗️ Data-driven buildings | Building height/style reflects stars, repo size, and activity |
| 🚗 Living atmosphere | Animated traffic, street lights, drifting fireflies, glowing beacon |
| 🔗 Shareable cities | Every city has a shareable link (`?user=username`) |
| 📱 Mobile-ready | Touch-friendly input, on-screen keyboard handling, responsive HUD |
| 🔒 No login, no backend | Uses GitHub's public REST API directly from the browser |

---

## Tech Stack

- **Rendering**: [Three.js](https://threejs.org) (WebGL 3D scene, lighting, fog, camera)
- **Frontend**: Vanilla HTML / CSS / JavaScript — zero build step, zero dependencies to install
- **Data source**: GitHub public REST API (`api.github.com`)
- **Fonts**: Space Grotesk, JetBrains Mono (Google Fonts)

---

## Getting Started

### Prerequisites

- A modern browser with WebGL support
- That's it — no Node, no package manager, no API key required

### Installation

```bash
git clone https://github.com/DevTropolis-city/DevTropolisCity.git
cd DevTropolisCity
```

### Running locally

It's a single static file, so any of these work:

```bash
# Option 1 — just open it
open index.html          # macOS
start index.html         # Windows

# Option 2 — serve it (recommended, avoids local-file CORS quirks)
python3 -m http.server 8000
# then visit http://localhost:8000
```

---

## Usage Examples

### Build a city from a username

Type a GitHub username (or a full profile URL) into the input and press **Build My City**:

```
torvalds
gaearon
sindresorhus
github.com/tj
```

### Share a city

Once built, the URL updates to `?user=<username>` — copy and share it directly, or use the in-app **Share** button.

---

## Project Structure

```
DevTropolisCity/
├── index.html                  # entire app: markup, styles, 3D scene, GitHub API logic
├── assets/
│   └── devtropolis_logo.png    # app logo / social preview image
├── .github/
│   ├── ISSUE_TEMPLATE/          # bug report & feature request templates
│   └── workflows/
│       └── deploy.yml           # GitHub Pages deploy workflow
├── .gitignore
├── CONTRIBUTING.md
├── CHANGELOG.md
├── SECURITY.md
├── LICENSE
└── README.md
```

---

## Deploying

Since it's a single static file, deploy it anywhere static hosting is supported:

- **GitHub Pages** — included workflow in `.github/workflows/deploy.yml` deploys `main` automatically to `https://devtropolis-city.github.io/DevTropolisCity/`. Or manually: Settings → Pages → deploy from `main` branch, root folder.
- **Netlify / Vercel** — drag-and-drop the folder, or connect the repo directly.

---

## Contributing

Contributions are welcome!

```bash
# Fork and clone
git clone https://github.com/YOUR_USERNAME/DevTropolisCity.git

# Create a feature branch
git checkout -b feat/your-feature-name

# Make changes, then open a PR
git push origin feat/your-feature-name
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

## License

MIT — see [LICENSE](LICENSE) for details.

---

## Links

- **Repo**: [DevTropolis-city/DevTropolisCity](https://github.com/DevTropolis-city/DevTropolisCity)
- **Live Demo**: [devtropolis-city.github.io/DevTropolisCity](https://devtropolis-city.github.io/DevTropolisCity/)
- **GitHub API docs**: [docs.github.com/rest](https://docs.github.com/en/rest)

---

Built with 🏗️ and ⚡ by [DevTropolis-city](https://github.com/DevTropolis-city) · Star ⭐ if you find it useful
