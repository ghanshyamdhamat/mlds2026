# MLDS 2026 — Static Course Website

This repository contains a simple static site for the Machine Learning for Data Science (MLDS) course. It is designed to be hosted using GitHub Pages.

## Structure

- `index.html` — Overview, prerequisites, highlights, Teams code
- `evaluation.html` — Evaluation plan and weights (from slides)
- `tutorials.html` — TA tutorials schedule and topics (from slides)
- `assets/styles.css` — Site styling (dark theme)
- `config/feature-flags.json` — Optional feature flags (see below)

## Run locally

You can preview locally using any static server, for example:

```zsh
# from the repo root
python3 -m http.server 8000
# then open http://localhost:8000
```

## Publish with GitHub Pages

1. Push this repository to GitHub.
2. In GitHub → `Settings` → `Pages`, set:
   - Source: `Deploy from a branch`
   - Branch: `main` (root)
3. Wait for deployment; your site will be available at the URL shown there.

## Feature flags (optional)

The file `config/feature-flags.json` demonstrates how to store a site-level feature toggle. It currently enables `GPT-5.1-Codex-Max` for all clients. You can extend this file as needed.