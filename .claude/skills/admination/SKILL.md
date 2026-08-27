---
name: admination
description: Admination system health check — verify sibling repos, knowledge base sync, active sessions, conventions, and installed tooling (MCPs/CLIs). Invoke by typing /admination.
---

Run the full Admination system health check now.

Load and follow the plugin skill `admination:admination` in this repo's context, and report its result verbatim — the green/yellow/red section summary with any red items and their fix commands listed first. Do not reimplement the checks here; the plugin skill is the single source of the doctor logic. If the plugin skill is unavailable, tell the user the admination plugin is not installed and point them at `/plugin` and the onboarding skill.