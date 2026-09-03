# JuliaData/DataFrames.jl context
> refreshed 2026-09-03 | upstream default: main @ d06ff9768ce91c5377d2c3625e7e1c7544208cc5

## Identity & policies
- upstream: JuliaData/DataFrames.jl, default branch main, primary language Julia, English-first: yes (docs/issues/README all English)
- CLA/DCO: none (no CLA bot, no DCO; policy passport cla_required=false, dco_required=false)
- AI-assisted PR policy: unstated (CONTRIBUTING.md has no AI disclosure requirement)
- signed commits required: no (no `required_signatures`, no verify-commit-signatures workflow)
- PR template: none (no .github/pull_request_template, pr_template_present=false)
- external tracker: GitHub only

## Conventions (verified from merged PRs)
- branch naming: no single dominant pattern — mixed `patch-N`, `feature/...`, `fix-*-error`, `bk-*`. Docs/link PRs used plain names (e.g. `Correct-link-to-XLSX-in-docs`). Use `docs/...` for a docs trivial pass.
- commit style: plain imperative subjects; not consistently Conventional Commits.
- test command: Julia `Pkg.test()` (run from repo root); docs build via `julia make.jl` from `docs/`.
- CI: GitHub Actions `ci.yml` (matrix of Julia versions, runs the full test suite).
- how outside PRs merge: responsive; many external docs/link/typo PRs merged (e.g. #3542 "Fix doubled word in indexing docs", #3531 "Update XLSX.jl link in docs", #3519 "Fix link for Data Wrangling Cheat Sheet", #3477 "typo, df was d", #3474 "Docs: Fix typo", #3384 "fix typos"). Merge cadence roughly monthly.

## Maintainer picture
- primary maintainer: Bogumił Kamiński (`bkamins`), commits daily; frequent PRs under `bk-*`/`bkamins-patch-N` branches.
- other active: `abhro` (recent docs/CI PRs #3545 #3544 #3543), community contributors merge often.

## Issue-area health
- docs/links area healthy: maintainers accept small docs/link/typo PRs from outsiders readily.
- avoid in-flight maintainer areas: internal refactors (`kc/...`, `bk-...`) — docs prose is safe ground.

## Gap ledger (dedupe — READ FIRST, never re-pick)
- 2026-09-03 trivial docs pass — pr-opened (fork PR #1) — 6 fixes/4 files: 2 typos (accidently, analagous), 2 broken links (GLM.jl /stable/manual/ 404, Tidier.jl /dev/ 404), 2 stale CONTRIBUTING build paths (doc/_build + docs/_build -> docs/build, confirmed by docs/build in .gitignore). No upstream PR touched these.

## Mined gaps (discovered, not yet attempted)
- (none pending)
