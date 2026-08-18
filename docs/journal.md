# Build Journal

Per-issue record of the unattended (Lane B) build of this project. One entry per Claude run, appended automatically by `.github/workflows/claude.yml` via `.github/scripts/journal-entry.sh`.

## How this file is written

**Entries are appended by the workflow, not by Claude inside its PR.** This is deliberate: having Claude append a journal entry within each PR means every open PR touches the same file, so almost every one goes `CONFLICTING` the moment any other PR merges — leaving green, auto-merge-enabled PRs sitting unmerged indefinitely. Patching from the workflow after the run sidesteps that entirely: Claude's branches never touch `docs/journal.md`.

## What "Estimated Cost" means

This pipeline authenticates via a **Claude subscription** (OAuth), not pay-per-token API billing. The cost figure is notional — what the run *would* cost at standard list rates — useful as a consistent yardstick for comparing runs, not an actual charge.

---

## Build velocity

Recomputed by `.github/scripts/journal-entry.sh` on every run.

<!-- VELOCITY_START -->
| Metric | Value |
|---|---|
| Issues with recorded metrics | 3 |
| Successful runs | 3 |
| Mean time per issue | 1m 57s |
| Mean turns per issue | 37 |
| Mean output tokens per issue | 8,819 |
| Mean estimated cost per issue | $0.1326 |
<!-- VELOCITY_END -->

---

## Entries

<!-- ENTRIES_START -->
<!-- New entries are appended below this marker, newest last. -->

## 2026-08-18 — Issue #2: M1: index.html and style.css — the hello page

- **Result:** success
- **PR:** #5
- **Milestone:** M1: The page
- **Model:** claude-sonnet-5
- **Execution Duration:** 76 seconds
- **Turns:** 32
- **Input Tokens:** 102
- **Output Tokens:** 4938
- **Estimated Cost:** $0.0744 (notional — see above)
- **Run:** https://github.com/mmorrow24work/ai-app-factory-hello-world-v4/actions/runs/32136864949

## 2026-08-18 — Issue #4: M3: about.html and README

- **Result:** success
- **PR:** —
- **Milestone:** M3: About page and README
- **Model:** claude-sonnet-5
- **Execution Duration:** 74 seconds
- **Turns:** 21
- **Input Tokens:** 60
- **Output Tokens:** 4660
- **Estimated Cost:** $0.0701 (notional — see above)
- **Run:** https://github.com/mmorrow24work/ai-app-factory-hello-world-v4/actions/runs/32145915323

## 2026-08-18 — Issue #4: M3: about.html and README

- **Result:** success
- **PR:** —
- **Milestone:** M3: About page and README
- **Model:** claude-sonnet-5
- **Execution Duration:** 201 seconds
- **Turns:** 59
- **Input Tokens:** 178
- **Output Tokens:** 16858
- **Estimated Cost:** $0.2534 (notional — see above)
- **Run:** https://github.com/mmorrow24work/ai-app-factory-hello-world-v4/actions/runs/32145910576
