# Repository Guidelines

## Project Structure & Module Organization
- Root pages: `index.html`, `summary.html` (primary entry points).
- Styles: `css/styles.css`.
- Scripts: `js/scripts.js`, `js/Timeline.js` (component-style JS).
- Assets: images in `assets/img/` and a few at root (e.g., `JoelHolmesProfilePic.jpeg`, `summary.jpeg`).
- GitHub Pages: `_config.yml` configures the site; `CNAME` sets the custom domain.

## Build, Test, and Development Commands
- Local preview (simple HTTP server): `python3 -m http.server 4000` then open `http://localhost:4000`.
- Quick check without a server: open `index.html` directly in a browser.
- GitHub Pages build: pushes to `main` are auto-deployed by Pages (no manual build step here).
- Optional Jekyll serve (if you have Jekyll installed): `jekyll serve --livereload` to emulate Pages locally.

## Coding Style & Naming Conventions
- HTML: semantic elements, 2-space indent; keep page-level HTML in root files.
- CSS: 2-space indent; group related rules; prefer utility classes over inline styles; keep styles in `css/styles.css`.
- JS: ES6+; avoid globals; keep site scripts in `js/scripts.js`. Use PascalCase for single-purpose modules (e.g., `Timeline.js`), kebab-case for multiword filenames otherwise.
- Assets: lowercase kebab-case for images under `assets/img/`.

## Testing Guidelines
- Manual smoke test: load pages in Chrome and Safari/Firefox; verify no console errors, links work, and layout is responsive.
- Visuals: confirm hero image, timeline, and summary sections render correctly on mobile and desktop.
- Accessibility: check headings order, alt text on images, and color contrast.

## Commit & Pull Request Guidelines
- Commits: concise, imperative mood (e.g., `fix: update profile summary`, `style: tweak timeline CSS`).
- PRs: include a short description, screenshots/GIFs for visual changes, and link related issues. Keep changes scoped; note any content edits.
- Before opening a PR: run a local preview and recheck links/navigation.

## Security & Configuration Tips
- Do not modify or remove `CNAME` unless changing the domain.
- Keep `_config.yml` minimal and consistent with GitHub Pages expectations; no secrets are stored here.
- Optimize images (dimensions/size) before committing to keep load times fast.

