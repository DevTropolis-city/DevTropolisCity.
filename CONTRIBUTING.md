# Contributing to DevTropolis

Thanks for considering a contribution! DevTropolis is a single-file, zero-build-step
project, so the bar to contribute is intentionally low.

## Ways to contribute

- 🐛 Report bugs via [Issues](../../issues)
- 💡 Suggest features via [Issues](../../issues)
- 🛠️ Submit fixes or improvements via Pull Request
- 📖 Improve documentation

## Development setup

No build step, no dependencies to install:

```bash
git clone https://github.com/YOUR_USERNAME/DevTropolisCity.git
cd DevTropolisCity
python3 -m http.server 8000
# open http://localhost:8000
```

Edit `index.html` directly — it contains all markup, styles, the Three.js
scene, and the GitHub API logic in one file.

## Making changes

1. Fork the repo and create a feature branch:
   ```bash
   git checkout -b feat/your-feature-name
   ```
2. Make your changes in `index.html`.
3. Test in a real browser — reload, try a few different GitHub usernames
   (including ones with very few or very many repos), and check mobile
   sizing if you touched layout or the 3D scene.
4. Commit with a clear message and open a Pull Request.

## Pull Request guidelines

- Keep PRs focused on one change where possible.
- Describe what changed and why in the PR description.
- Include a screenshot or short clip if the change is visual.
- Be patient — this is a side project maintained in spare time.

## Code style

- Vanilla JS, no framework, no build tooling — please keep it that way.
- Match the existing naming and structure conventions in `index.html`
  (HUD elements prefixed `hud-`, search-screen elements prefixed `sc-`/`ss-`, etc).
- Favor small, readable functions over clever one-liners.

## Reporting bugs

When filing a bug, please include:

- Steps to reproduce
- Expected vs actual behavior
- Browser + OS
- The GitHub username you tested with, if relevant
