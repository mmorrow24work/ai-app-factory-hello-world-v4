# ai-app-factory-hello-world-v4

Create a simple hello-world site to test the ai-app-factory build process Built and evolved via the unattended (Lane B) Claude Code pipeline: label an issue `claude-go` and `.github/workflows/claude.yml` implements it, opens a PR, and records the run in `docs/journal.md`.

This is a **disposable factory test, not a maintained project** — it exists to exercise
the `ai-app-factory` pipeline, and its content is not the point.

## Live site

<https://mmorrow24work.github.io/ai-app-factory-hello-world-v4/>

## Viewing locally

Open `index.html` in a browser. Note that a plain `file://` open serves the page from the
filesystem root, not from the `/ai-app-factory-hello-world-v4/` subpath the site is actually
deployed under on GitHub Pages — so a relative-path bug that would 404 in production can
still look fine locally. Serving the repo root over HTTP (e.g. `python3 -m http.server`) and
browsing to the page under a subpath is closer to production, though not identical.

## Requested by

[@mmorrow2012](https://github.com/mmorrow2012), via [ai-app-factory](https://github.com/mmorrow24work/ai-app-factory).

## Support & Handoff

### Support

Open an issue, or comment on an existing one:

- Apply the `claude-go` label (or comment `@claude`) to have the unattended pipeline attempt a fix.
- Mention `@mmorrow24work` for anything the pipeline can't or shouldn't handle unattended — design decisions, ambiguous requirements, anything labeled `lane:manual`.

### Handoff

Once this project's milestones are complete, fork the repo to take ownership.

GitHub forks do **not** inherit the parent repo's Actions secrets, so `claude-go` stops working on the fork the instant it's created — no separate revoke step needed on the original owner's side. To keep the unattended pipeline running, the new owner sets up their own `CLAUDE_CODE_OAUTH_TOKEN`/`GH_PAT` secrets on their fork (same `claude setup-token` / `gh secret set` steps documented in the `ai-app-factory` repo's own `README.md`).
