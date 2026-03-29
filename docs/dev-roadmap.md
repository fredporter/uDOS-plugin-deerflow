# Development Roadmap

## Phase 0 - Scaffold
- create adapter repo
- define schemas
- add clone and update scripts
- establish compatibility matrix
- add minimal translator, executor, validator stubs

## Phase 1 - Translation MVP
- support linear workflows
- support dependencies and fan-out
- map basic tool and prompt steps
- produce deterministic graph output
- snapshot test translation results

## Phase 2 - Execution MVP
- invoke local Deer Flow clone
- stage runtime directories
- capture logs and outputs
- normalize success and failure results
- support dry-run and validation modes

## Phase 3 - Policy integration
- trust profiles
- path restrictions
- network profiles
- skill allowlist
- upstream version gating

## Phase 4 - Wizard lane
- expose adapter as a wizard-selectable execution backend
- add visualization and inspect modes
- support long-horizon agent workflows

## Phase 5 - Certified workflow set
- publish supported workflow classes
- conformance tests
- benchmark cost and runtime
- promote selected lanes to certified

## Deferred
- full visual graph builder
- bidirectional graph editing
- memory sync import/export
- production remote cluster execution
