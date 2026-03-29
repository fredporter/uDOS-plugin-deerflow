# uDOS-plugin-deerflow

uDOS-plugin-deerflow is the optional Deer Flow execution adapter lane for the
uDOS family.

It is an experimental backend for translation and controlled execution of
graph-heavy or long-horizon workflows, without moving canonical workflow truth,
vault persistence, publish routing, or certification boundaries out of uDOS.

## Boundary

uDOS remains the authority for:

- `#binder` semantics
- workflow source of truth
- compile contracts
- vault persistence
- publish routing
- MCP policy and trust classes
- certification boundaries

Deer Flow is used as:

- a cloned upstream dependency
- an optional graph execution surface
- an advanced runtime for long-horizon or multi-step tasks
- a tool and sub-agent execution engine
- a sandboxed experimental lane for power workflows

## Activated Surfaces

- stable docs under `docs/`
- translation and result schemas under `schemas/`
- adapter and executor stubs under `src/python/`
- graph helper stubs under `src/ts/`
- validator stub under `src/go/`
- upstream bootstrap and sync helpers under `scripts/`
- repo validation entrypoint under `scripts/run-deerflow-checks.sh`

## Why Clone, Not Fork

This plugin expects Deer Flow to be cloned as an upstream-managed dependency,
not permanently forked into a divergent product repo.

That keeps update flow cleaner:

1. clone upstream Deer Flow
2. pin a tested commit or tag in uDOS
3. apply adapter-side translation and orchestration in this repo
4. periodically pull upstream changes and re-run conformance checks

## Validation

Run:

```bash
bash scripts/run-deerflow-checks.sh
```
