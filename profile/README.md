# Quattro Commas ♛

**A verification-gated AI studio.** Applied ML and agent tools that carry their own evidence — and the gates that make them checkable.

Run by [Kiliaan Vanvoorden](https://github.com/BoozeLee) from a plant-filled loft in Riemst, Belgium. Ideas, code, culture, freedom.

We publish failure states unprompted. A guard that has never been watched to fail has not been shown to work — `elohim` ships tampered copies of its own instruments, and every project under this org publishes its own broken-on-purpose check that runs on every invocation.

**Open to AI engineering roles** in evaluation and agent infrastructure — remote from Belgium, employment or contract.
📧 [bakerstreetbandit@zohomail.eu](mailto:bakerstreetbandit@zohomail.eu) · [one-page CV](https://quattro-commas.github.io/resume.pdf) · [Site](https://quattro-commas.github.io)

## The four commas

> `,` Ideas · `,` Code · `,` Culture · `,` Freedom

## What we build

- **Agent systems** — multi-agent tooling, MCP servers, CLI/TUI engineering agents
- **Evaluation gates** — deterministic checksum-gated measurement; tamper tests that must fail
- **Local inference** — local-first LLM tooling, Ollama pipelines, sidecar architectures
- **Applied ML** — industrial computer vision and yield-prediction experiments for food processing

## House rules

- Every number in a README is re-derivable from the repo or from a recorded measurement.
- A claim we could not read is `UNKNOWN`. It is never `FALSE`, and never an all-clear.
- A confirmed defect is pinned as a failing test, not quietly fixed.
- A repository says what it cannot do.

## What we do not claim

- No customer count, revenue, or funding. None.
- No production deployments — there is nothing running for anyone but us. This is a measurement, not an ambition.
- No claim that our gates cover the applied-ML repositories, which are private and unreviewed.
- No guarantee against the owner rewriting history — audits come from re-deriving each claimed number against a fresh clone of the relevant repo, not from any promise that this README will always reflect the live project state.

## Where the code is

This org is the studio's index — identity, thesis and distribution. The implementation lives in the public
repositories below, maintained and built by the same one person. Built by one person means you know who answers
for a broken gate — not that the work is small. Nothing here is a mirror or a fork.

The portfolio is **five** public repositories plus this index: `elohim`, `harness`, `terminal221b`,
`mcp-regression-lab` and `repotruth`. Re-derive the count with
`gh repo list BoozeLee --limit 100 --json name --jq '.[].name'`.

| Project | What it gates | Language | Licence |
|---|---|---|---|
| [**elohim**](https://github.com/Quattro-Commas/elohim) | Numerical claims — publishes a number only when it can re-derive it | Python | MIT |
| [**harness**](https://github.com/Quattro-Commas/harness) | Agent edits — blocks protected-path writes and secret reads before an edit lands | Python | AGPL-3.0 |
| [**terminal221b**](https://github.com/Quattro-Commas/terminal221b) | A local-first coding CLI, bounded to a workspace | TypeScript, Rust | AGPL-3.0 |
| [**mcp-regression-lab**](https://github.com/Quattro-Commas/mcp-regression-lab) | MCP tool contracts — a renamed or narrowed tool fails CI instead of production | TypeScript | ISC |
| [**repotruth**](https://github.com/Bakery-street-project/galacticfederation) | CI that reads the repository, not just the diff. A personal project, so it is hosted outside this org | TypeScript | AGPL-3.0 |

## Current state — stated, not hidden

Five of five public repositories are accounted for above. Re-verified **2026-10-11**: the four showcase
repos (`elohim`, `harness`, `terminal221b`, `mcp-regression-lab`) all have **green CI** on their latest
runs. `repotruth` is maintained outside this org at `Bakery-street-project/galacticfederation`.

Every project sits at **0 stars and 0 forks**. There are no customers and no deployments.

## Private work, shown on request

The applied-ML and local-inference work runs in private repositories and will not be published, so no client,
dataset or repository name appears here — and no metrics are quoted, because none of them can be
re-derived from a public repo. What can honestly be described is the shape of it, which is the only
evidence behind the applied-ML and local-inference pillars above:

- a multi-task image classifier that takes one photo and returns both a class and a storage-age estimate, served from ONNX behind FastAPI with a browser demo in front of it
- a lot-level yield predictor that routes output to specification tiers
- a shelf-life-aware allocation advisor (FIFO/FEFO) paired with a local-first store assistant
- a Next.js chat copilot wired to internal tooling over MCP
- a MAP-Elites quality-diversity search over idea spaces

All of it is screen-shareable on request.

## Thesis

> A guard that does not hold must fail the run.

Collected and explained in [`eval-gates`](https://github.com/Quattro-Commas/eval-gates).