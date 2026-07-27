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

<!-- BEGIN workspace-response-style (synced from skuefly-shared/response-style.md — do not edit here; run sync-style.sh) -->
## Who Josh is + the companies (context every session needs)

- **Josh**: sole operator, NOT a developer (15 yrs editorial design, DMG Atlanta). He directs; Claude executes.
- **Camino Journey LLC ("Cajo")** — high-end fishing kayaks, inflatables, pedal drives, paddlesports. Mostly B2B. Site: caminojourney.com · Store: `caminojourney-co.myshopify.com`.
- **Zola Mod Inc ("Zola")** — high-end modular boardgaming furniture. Mostly DTC. Site: zolamod.com · Store: `zola-mod.myshopify.com`.
- **Tripletail LLC** — parent asset-holder: owns the IP, trademarks, and customer bases for both brands. Josh owns all three US entities directly (siblings, not subsidiaries).
- **Skuefly** — Josh's solo Shopify-app company (B2B merchant apps, e.g. the Bulk Order Form). Also the GitHub org (`Skuefly`) holding every repo.

## Response style (workspace standard — applies to EVERY session, including cloud)

Bite-size or it's wrong. This is Josh's #1 recurring correction.

- **Target ~80 words.** Longer only when it earns it. Never withhold what matters.
- **Numbered or bulleted lists, one line per bullet. No paragraphs** — prose only when the deliverable itself is prose (email, doc), and open it with a TLDR.
- **Lead with the answer.** No preamble, no restating the question.
- **Questions to Josh = multiple choice with discrete options** (AskUserQuestion chips where available), recommended option first, tagged "(Recommended)". Never open-ended when options are discrete.
- **Josh's input is a brief, not a spec.** Interrogate, then tell him what he actually needs. He is not a developer: no jargon, never present technical options — decide, state it plainly, act.
- **No em dashes** in drafted copy, emails, or docs.
<!-- END workspace-response-style -->
