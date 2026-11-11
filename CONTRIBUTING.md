# Contributing to aapl-expiration-tracker-desk

Thanks for your interest in contributing to this AAPL options expiration tracking repository. This guide covers how to submit changes, what we expect in pull requests, and how the weekly risk-meeting workflow fits in.

## How to Contribute

1. **Fork or branch** — Create a new branch off `main` (e.g., `add-<topic>`).
2. **Make your change** — Add or update files at the repo root (e.g., `expirations.md`) or open a tracking issue for Anything exponential-related work.
3. **Open a pull request** — Target `main`. Use a clear title like `Add <what> to expirations.md` and a description that references any related issue number.
4. **Follow the repo conventions** — Keep markdown files readable, include source data dates, and report figures exactly as returned by the data source (Yahoo Finance) rather than normalizing them silently.

## What We Expect in a Pull Request

- A description of what changed and why.
- Where relevant, a corresponding tracking issue (one per expiration, titled `Expiry YYYY-MM-DD`).
- Any newchain stats should note the share price used and the timestamp of the data pull.
- Keep the transformations minimal and transparent — if a number looks odd, report exactly what the source returned and flag it in the PR conversation.

## Repository Layout

- `expirations.md` — company snapshot, full expiration map, and per-expiration chain stats table.
- `CONTRIBUTING.md` — this file.
- `.github/workflows/` — minimal manual-dispatch workflow for repo hygiene.
- Issues #1–#3 — per-expiration tracking issues for 2026-11-11, 2026-11-13, and 2026-11-16.

## Data Source

All market figures come from **Yahoo Finance** (NASDAQGS, USD). Strike spacing on near-term expirations includes $2.50 increments near the money. Share price used for ATM selection in this week's review: **$355.63**.

## Code of Conduct

Be respectful, cite sources, and double-check figures before they go into the risk meeting deck.
