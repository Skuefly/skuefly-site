# Skuefly Website

## Overview
Static website for Skuefly. Hosted on GitHub Pages.

## Hosting
- **Domain:** skuefly.com
- **Hosting:** GitHub Pages (from `main` branch)
- **Repo:** skuefly/skuefly-site

## Structure
- `index.html` — Main landing page
- `help/` — Help documentation
- `privacy/` — Privacy policy
- Favicon and icon assets in root

## Deploy
Push to `main` → GitHub Pages auto-deploys. No build step needed.

## Cloud Environment (Claude Code on the Web)
If you cannot push directly to `main`:
1. Create a branch with the `claude/` prefix (e.g., `claude/fix-scroll-issue`)
2. Push that branch — a GitHub Action will auto-merge it to `main`
3. Do NOT create PRs — the auto-merge handles deployment

The `claude/` branch prefix is required for auto-merge to trigger.
