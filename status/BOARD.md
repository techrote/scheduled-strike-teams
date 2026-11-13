# Campaign status board — snapshot

**Snapshot time:** 13 November 2026, initial repository setup.  
**Authoritative live coordination:** [campaign #1](https://github.com/techrote/scheduled-strike-teams/issues/1) and the linked team issues.  
**No new campaign schedules have been created or enabled by repository bootstrap.**

## Capacity and health

| Indicator | Last recorded | Evidence/status |
| --- | --- | --- |
| Maximum hourly slots | 10 | Owner-set global campaign cap |
| Enabled tasks found before setup | 1 | ShadeDoomVK CI A/B monitor; recheck before activation |
| Remaining potential slots | 9 | Only if active schedule list remains unchanged |
| Proposed worker slots | 9 | Seven campaign teams, **not yet activated** |
| Active campaign worker IDs | None recorded | No schedules launched yet |
| Verified scoped READY_OWNER transitions | 0 **recorded by this campaign** | Baseline does not invalidate earlier repo qualifications |
| Human gates | sandimations Pages, flatCAD editorial, Windows acceptance | [owner queue #9](https://github.com/techrote/scheduled-strike-teams/issues/9) |

## Team lanes

| Rank | Team issue | Proposed worker slots | State | Current first target | Exact-head qualification / next milestone |
| ---: | --- | ---: | --- | --- | --- |
| 1 | [Greygen #2](https://github.com/techrote/scheduled-strike-teams/issues/2) | 2 | **CANDIDATE** | [greygen #46](https://github.com/techrote/greygen/issues/46), [#47](https://github.com/techrote/greygen/issues/47) | Actual Pages-path browser CI and icon/install matrix |
| 2 | [HWiNFOterm #3](https://github.com/techrote/scheduled-strike-teams/issues/3) | 1 | **CANDIDATE** | [PR #1](https://github.com/techrote/HWiNFOterm/pull/1) | Exact-head Windows/Linux CI, explicit physical acceptance |
| 3 | [INTUIT3D #4](https://github.com/techrote/scheduled-strike-teams/issues/4) | 1 | **CANDIDATE** | [PR #351](https://github.com/techrote/INTUIT3D/pull/351) | Wrong-body cut semantics, Ubuntu+Windows CI |
| 4 | [Steelmoth #5](https://github.com/techrote/scheduled-strike-teams/issues/5) | 2 | **CANDIDATE** | [PR #121](https://github.com/techrote/steelmoth/pull/121), [#124](https://github.com/techrote/steelmoth/pull/124), [#119](https://github.com/techrote/steelmoth/pull/119) | Independent review, dependency-order reconcile |
| 5 | [DashMinimix #6](https://github.com/techrote/scheduled-strike-teams/issues/6) | 1 | **CANDIDATE** | [PR #18](https://github.com/techrote/DashMinimix/pull/18) | Exact-head source-switch preservation regressions |
| 6 | [Flexdiffusion #7](https://github.com/techrote/scheduled-strike-teams/issues/7) | 1 | **CANDIDATE** | [PR #9](https://github.com/techrote/flexdiffusion/pull/9) | Alpha extraction UI/regression handoff |
| 7 | [Omnipanel #8](https://github.com/techrote/scheduled-strike-teams/issues/8) | 1 | **CANDIDATE** | [PR #90](https://github.com/techrote/omnipanel/pull/90) | Exact-head workflow tests; #89 remains open |
| — | Existing ShadeDoomVK monitor | 1 | **ENABLED AT LAST CHECK** | CI A/B results | Stop after evidence; not newly created by this campaign |

These slots total ten **only if all proposed workers are subsequently enabled while the existing monitor remains active**. Actual enabled count is the source of truth, not this table.

## Owner action / zero-worker lanes

| Priority | Project | Action | Link |
| --- | --- | --- | --- |
| Urgent unblock | sandimations | Enable GitHub Pages if missing; then one worker can finish live deploy | [PR #22](https://github.com/techrote/sandimations/pull/22) · [owner queue](https://github.com/techrote/scheduled-strike-teams/issues/9) |
| Quick editorial | flatCAD | Owner review of Beta 1 docs-only PR | [PR #32](https://github.com/techrote/flatCAD/pull/32) |
| Manual hardware | HWiNFOterm | Live HWiNFO + Windows Terminal acceptance | [PR #1](https://github.com/techrote/HWiNFOterm/pull/1) |
| Manual runtime | INTUIT3D | Windows wrong-body/valid-cut evaluation | [PR #351](https://github.com/techrote/INTUIT3D/pull/351) |

## Review log

- **2026-11-13 — Setup.** Campaign repository initialized, seven potential teams and owner gate documented. No campaign worker started. First real orchestration update must refresh the task inventory and annotate each team's actual worker ID and source SHA.
- **Next review:** update this board only after inspecting team issue receipts and target repo evidence. The separate campaign issue is the live audit trail; do not erase previous dated milestones.

## Board update rules

Make small, dated changes. Never mark a team ACTIVE without its actual enabled automation ID(s), READY_OWNER without exact SHA/CI/acceptance evidence, or COMPLETE merely because a PR is marked mergeable. Keep owner approval and release state explicit. Retire old workers promptly; do not recycle team issue identity for unrelated projects without documenting the change.
