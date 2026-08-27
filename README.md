# SpaDES.ai

Shared conventions, guidelines, and skills for AI-assisted development on the
**SpaDES toolkit** — the R packages that implement Spatial Discrete Event Simulation
(`SpaDES.core`, `SpaDES.tools`, `SpaDES.project`, `reproducible`, `Require`, and their
companions).

This repository is the team's single source for how to work with a
Posit-Assistant-enabled Claude model on the SpaDES toolkit packages and related code.
It holds three things:

- **`guidelines/`** — path-agnostic setup and convention docs. Start at
  [`guidelines/00-user-setup.md`](guidelines/00-user-setup.md); the reference docs are
  `00b-user-guidelines.md` (working *with* the assistant), `01-project-setup.md`
  (project folder + repo set), `02-guardrails.md` (permissions, hooks, `AGENTS.md`),
  and `03-skills.md` (getting, creating, and loading skills).
- **`AGENTS.md`** — a template project-memory file to copy into a SpaDES workspace root
  and adapt (paths, repository set) to that workspace.
- **`skills/`** — the shared team skills (`spades-*`). These are the primary source;
  get them before writing new ones.

## Getting the skills

Clone or sync this repo into a local skills path so Posit Assistant discovers the
skills, e.g. `~/.agents/skills` or `~/.posit/assistant/skills/`. See
[`guidelines/03-skills.md`](guidelines/03-skills.md) for details and precedence rules.

## Shared vs local

The docs here are **shared and path-agnostic**. Machine-specific records (concrete
paths, installed config) are kept as **local instances** — files named `*.local.md`
that stay out of this repo. See the "Local instances of these guidelines" section in
[`guidelines/00-user-setup.md`](guidelines/00-user-setup.md).

## Related work

[LandR.ai](https://github.com/CeresBarros/LandR.ai) is an **example** of a SpaDES-based
system (the LandR module/model ecosystem) that has built its own AI-assisted-development
support docs and tools. SpaDES.ai is the toolkit-focused sibling: it targets the
SpaDES *toolkit packages* rather than LandR modules, and is self-contained — it does not
depend on LandR.ai.

---

The documents in this repository — this README, the `guidelines/`, the `AGENTS.md`
template, and the `skills/` — were drafted with assistance from Claude (Posit Assistant).
