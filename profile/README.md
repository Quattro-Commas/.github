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
- No guarantee against the owner rewriting history — `orgmind`'s `SECURITY.md` states the limit exactly.

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

Five of five public repositories are accounted for above. Re-verified **2026-10-08**: **no project is
failing a test.** `elohim` is green on its latest run.

One real defect exists and it is older than it looks: `harness` last *executed* CI at commit `d11de009` on
2026-10-02 and failed on `uv sync --frozen`. The six commits since include
`0eebe594 "Repair uv.lock after the harness-agent2 rename"`, which is very likely its fix — but that fix has
never been validated. `harness` is **probably green and unverified**, not green.

`terminal221b` and `repotruth` are in the same position: their most recent red runs are not test results.
Neither has an executed run on `main` since the billing refusals began, so their current state is `UNKNOWN`,
not green. `repotruth` also has one `startup_failure` (2026-10-05) with no job record at all.

Every project also sits at **0 stars and 0 forks**. There are no customers and no deployments.

### Why the checks are red, and what that does not mean

The last runs on `harness`, `terminal221b`, `mcp-regression-lab` and `repotruth` all failed **without
executing a single step** — no runner was ever assigned. GitHub refused to start them:

> The job was not started because recent account payments have failed or your spending limit needs to be
> increased.

That is a billing refusal, not a test result. A job with no steps never ran a line of the code, so it
cannot be evidence about the code. Read the conclusions without this distinction and you get the tidy,
wrong, flattering-of-nobody answer that most of the portfolio was red — which describes a GitHub invoice, not
code.

`mcp-regression-lab` is the clearest case: its last executed run, CodeQL on 2026-10-03, **succeeded**. The
red run that followed it on 2026-10-05 ran no steps.

Re-derive the check state yourself. A run counts only if a job actually executed steps:

```bash
sh qc-work/check-state.sh
```

That script prints one line per failing job with its `steps=` count and `runner`, so the billing refusals are
visible instead of silently counted. Note that `repotruth` is **not** under this account — it lives at
`Bakery-street-project/galacticfederation`, so pass that name explicitly:

```bash
sh qc-work/check-state.sh Quattro-Commas/elohim Quattro-Commas/harness Quattro-Commas/terminal221b \
  Quattro-Commas/mcp-regression-lab Bakery-street-project/galacticfederation
```

`steps=0` with an empty `runner` is the billing-refusal signature, and it is the thing to filter out.

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