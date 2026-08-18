# AGENTS.md

## Cursor Cloud specific instructions

This repository is a single, dependency-free static website (Team Topnotch LLP). There is **no build system, package manager, test suite, or lint tooling** — it is plain HTML/CSS/JS.

- Entry point: `index.html` at the repo root. Standalone design showcases live in `showcase/`. Static assets (WebP images, `logo.svg`) live in `assets/`.
- Run (development): serve the repo root as static files, e.g. `python3 -m http.server 8000`, then open `http://localhost:8000/index.html`. Opening `index.html` directly via `file://` also works but relative asset paths and the `mailto:` action are best verified over HTTP.
- Build: none required. Deployment is just uploading `index.html`, `robots.txt`, and `assets/` as-is (see `README.md`).
- Tests / lint: none exist in the repo. Do not fabricate a framework; validate changes by loading the page in a browser.
- Interactive functionality is all client-side: the mobile nav toggle and the enquiry form (`#enquiryForm`). The form calls `event.preventDefault()` and builds a `mailto:teamtopnotch.llp@gmail.com` link, so submitting it opens the OS mail-application chooser rather than posting to a server — that dialog is expected, not an error.
