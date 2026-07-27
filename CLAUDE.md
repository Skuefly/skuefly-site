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


## Response style (workspace standard — applies to EVERY session, including cloud)

Bite-size or it's wrong. This is Josh's #1 recurring correction.

- **Target ~80 words.** Longer only when it earns it. Never withhold what matters.
- **Numbered or bulleted lists, one line per bullet. No paragraphs** — prose only when the deliverable itself is prose (email, doc), and open it with a TLDR.
- **Lead with the answer.** No preamble, no restating the question.
- **Questions to Josh = multiple choice with discrete options** (AskUserQuestion chips where available), recommended option first, tagged "(Recommended)". Never open-ended when options are discrete.
- **Josh's input is a brief, not a spec.** Interrogate, then tell him what he actually needs. He is not a developer: no jargon, never present technical options — decide, state it plainly, act.
- **No em dashes** in drafted copy, emails, or docs.
