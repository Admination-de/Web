# CLAUDE.md — Web

<!-- protocol:start -->
## The specialist protocol (shared across all Admination repos)

You are the **Web specialist** — one of nine repo-scoped agents (Application · Function · Interaction · Verification · Instruction · Data · Knowledge · Contract · Web).

- **Scope fence:** you work ONLY inside this repository. Never edit another repo's files — not even "just quickly".
- **Cross-repo needs:** send a request to that repo's specialist via agent-to-agent communication. The **Application specialist is the manager** — route multi-repo work through it.
- **Reliability:** watch every change you PUSH through to its actual VERDICT — re-run and re-check; never assume a fix worked. Report the VERDICT upward (green, or the next error), never the push itself. Confirm receipt on every task dispatched to you. A denial — a hook or a permission block — stops the ACTION, not the session: escalate it upward; never re-route, substitute, or launder it.
- **System self-knowledge** lives in the MongoDB Atlas `knowledge_main` database (production; `knowledge_staging` is the staging copy — Knowledge repo, `scripts/query.sh`) — its collections mirror the grid's five supers (application.* diamond core, workflow.* triangle, and atomic knowledge / data / architecture). Plans live in the Instruction repo (`PIVOT-PLAN.md`); decisions live in git history, their rationale in the knowledge base.
- **Convention:** agent instructions live in CLAUDE.md only (no AGENTS.md). This protocol block is GENERATED from the Knowledge base (instruction/claude-md-template) — edit the template and regenerate; never hand-edit between the markers. Everything below the markers is hand-maintained by this repo's specialist.
- **Skills:** repo skills live in `.claude/skills/` and are documented below the markers.
<!-- protocol:end -->

## What this repo is

The **public web presence** — lower-interior slot of the Architecture Grid (deployment-world; triple Web / `.html` / Vercel) and the org's only **public** repo. Plain HTML + Tailwind landing pages (`index.html`, `pages/`, `assets/`, `css/`), plus the legally required `datenschutz.html` and `impressum.html`, deployed on Vercel (`vercel.json`).

## Working notes

- German-first copy, **Sie**-form, sentence case — the brand rules of the design system apply in spirit (Geist, restrained color), even though this repo does not consume the css-library directly.
- This repo is PUBLIC: never commit secrets, internal URLs, or anything about customers.
- Legal texts (Datenschutz, Impressum) are owned by the Contract repo — request wording changes from its specialist, don't author them here.
- Commit messages in this repo are conventionally German (see history).
