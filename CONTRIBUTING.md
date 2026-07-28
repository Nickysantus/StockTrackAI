# Contributing to StockTrackAI

This is a short guide so everyone on the team knows how we work together during the hackathon. It's intentionally simple — we're optimizing for speed and clarity, not process overhead.

## Roles & Ownership

- **Jezreal** — owns the backend and drives the native.builder build sessions. If you're touching backend logic or the native.builder workspace, coordinate with him first.
- **Abdoul Rahim** — owns the AI parsing agent, working alongside Jezreal.
- **Kamso Daniel & Inertia** — own the frontend/dashboard UI, plus the demo video and pitch deck.
- **NickySantus** — supervises, reviews, and handles final submission. Not writing code directly, but reviewing all merges into `main`.

## Branching

- Do **not** push directly to `main`.
- Create a branch off `main` for your work, named clearly:
  - `feature/dashboard-alerts`
  - `feature/parsing-agent`
  - `fix/debt-calculation`
- Keep branches focused — one feature or fix per branch, not a mix of unrelated changes.

## Commits

- Write clear, short commit messages describing *what changed*, not just "update" or "fix":
  - Good: `Add low-stock alert threshold logic`
  - Avoid: `changes`, `update 2`, `fix stuff`
- Commit often. Small, frequent commits are easier to review than one giant commit at the end.

## Pull Requests

- Open a PR when your branch is ready for review — don't wait until everything is "perfect."
- In the PR description, briefly note:
  - What this changes
  - How to test it (if applicable)
  - Anything you're unsure about
- Tag **@Nickysantus** or Jezreal for review before merging into `main`.
- Small PRs are easier to review quickly — if a change is large, consider splitting it.

## Communication

- Post quick updates in the WhatsApp group when you start and finish a meaningful chunk of work — this keeps everyone (especially Nicky, who's supervising) in the loop without needing a call.
- If you're blocked on something, say so early rather than waiting — someone on the team can likely help or unblock you.
- No fixed calls unless Jezreal flags one as necessary. Default to async, text-based updates.

## Native.builder Workflow

Since native.builder handles the actual generation and deployment:
- Jezreal drives the primary build sessions.
- Abdoul works directly with Jezreal on the AI agent layer within the same workspace.
- If you need access to the native.builder workspace and don't have it, ask Jezreal directly.
- Any exported code or config that needs to live in this repo should be committed after each meaningful milestone (not just at the end), so we always have a recoverable snapshot.

## Before the Deadline

Refer to the submission checklist in `docs/kickoff-brief.md`. Everyone is responsible for confirming their piece is done and pushed before the final 24 hours — don't leave it to the last minute.

## Questions

If anything here is unclear, ask in the group. This document can and should be updated if our workflow changes.
