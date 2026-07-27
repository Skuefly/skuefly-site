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
- **HARD RULE — kickoff protocol: survey before building.** Starting anything new (app, UI, pipeline, integration): FIRST lay out the efficient paths — existing kits/libraries/templates/services and in-house assets (admin UIs: the `@skuefly/ui` package + design system) vs scratch-building — recommend one, and sketch the full lifecycle (deploy, auth, rollout) up front so no step surfaces days in. Josh can't know what exists; hours of hand-rolling something the ecosystem ships is a failure.
- **HARD RULE — but architecture, guardrails, and policy get chips FIRST.** Changes to security rules, approval gates, risk tiers, unattended execution, or standing workflow policy: present multiple-choice options and wait for Josh's pick BEFORE writing or pushing anything. Technical implementation is Claude's call; policy is Josh's.
- **No em dashes** in drafted copy, emails, or docs.
- **Recaps, status reports, and briefings = compact tables in chat.** Josh is visual and absorbs fast: table cells ≤ 8 words, bold names, categorized sections — never prose paragraphs, never an artifact when a table in chat does the job.
- **Web-task instructions = deep links + numbered steps.** When Josh must do something in a browser himself: link the EXACT page (never the site home), one action per numbered step, name the precise button/field labels, call out the gotcha most likely to trip him (e.g. "the two keys sit next to each other"), and end with how he'll know it worked.

## The re-entry board (every session)

`OPEN-PROJECTS.md` on `main` of `Skuefly/skuefly-shared` is where every project's
"where it left off / next action / open questions" lives. **Before ending a session that
did real work, update your project's row** (cloud sessions: via gh / the GitHub API).
When Josh asks "where did I leave off?", read that board plus the repo's own
STATUS/HANDOFF and answer in 5 bullets or fewer. A stale row strands Josh — he juggles
many projects and this board is how he re-enters.

Two hard rules for the board:
- **Rows are written in Josh's language** — what the thing is in business terms and what
  he can do next ("say X in any session"), never PR/repo jargon (park identifiers in
  trailing parentheses for sessions).
- **Ideas must not evaporate.** If a conversation births an idea or exploration that
  doesn't become a repo/task by session end, PARK it under "Ideas & conversations" with
  one line + where the conversation lives. Capturing is the session's job, never Josh's
  discipline. "Make it a project" promotes it.

## Machine-bound or browser-bound work (cloud sessions)

If a task needs Josh's machine (local creds, flyctl, deploys) or a driven browser
(account provisioning, console setup): do NOT walk Josh through tutorials. Propose a
**handoff** — push `proposed/<id>.md` to the `handoffs` branch of `Skuefly/skuefly-shared`
(protocol + risk tiers in `handoffs/README.md` on that branch). Josh approves with
"run <id>"; his local Claude executes and reports back in `done/`.
<!-- END workspace-response-style -->
