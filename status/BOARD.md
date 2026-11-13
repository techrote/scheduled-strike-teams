# Campaign status board — snapshot

**Snapshot time:** 13 November 2026, after Flexdiffusion team activation (~17:45 UTC).  
**Authoritative live coordination:** [campaign #1](https://github.com/techrote/scheduled-strike-teams/issues/1) and the linked team issues.  
**Three Flexdiffusion workers have now been created and confirmed enabled.** See [TEAM-06 #7](https://github.com/techrote/scheduled-strike-teams/issues/7) for actual schedule IDs.

## Capacity and health

| Indicator | Last recorded | Evidence/status |
| --- | --- | --- |
| Maximum hourly slots | 10 | Owner-set global campaign cap |
| Enabled tasks verified after Flexdiffusion launch | **4** | Flexdiffusion A/B/C + ShadeDoomVK CI A/B monitor |
| Remaining available slots at last check | **6** | Recheck active task list before further assignment |
| Initial proposed worker slots | 9 | Three Flexdiffusion workers activated, six other proposed slots still unassigned |
| Active campaign worker IDs | **3** | A: `6af74cbd1a788191be877e450ca62333`; B: `6af74cbef05c8191b3cf5686b18d0858`; C: `6af74cc186bc8191aec39f3f19f65bad` |
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
| 6 | [Flexdiffusion #7](https://github.com/techrote/scheduled-strike-teams/issues/7) | **3** | **ACTIVE (3)** | [PR #9](https://github.com/techrote/flexdiffusion/pull/9), [#8](https://github.com/techrote/flexdiffusion/pull/8), [#10](https://github.com/techrote/flexdiffusion/pull/10) | A: inpainting; B: sampler; C: Blend Lab. Each 48 hourly runs, owner-gated handoff |
| 7 | [Omnipanel #8](https://github.com/techrote/scheduled-strike-teams/issues/8) | 1 | **CANDIDATE** | [PR #90](https://github.com/techrote/omnipanel/pull/90) | Exact-head workflow tests; #89 remains open |
| — | Existing ShadeDoomVK monitor | 1 | **ENABLED AT LAST CHECK** | CI A/B results | Stop after evidence; not newly created by this campaign |

**Capacity now verified: 4/10 enabled, 6 free.** Table mixes currently active Flexdiffusion with still-proposed slots; do not add all rows to infer live occupancy. The enabled automation list is the source of truth.

## Owner action / zero-worker lanes

| Priority | Project | Action | Link |
| --- | --- | --- | --- |
| Urgent unblock | sandimations | Enable GitHub Pages if missing; then one worker can finish live deploy | [PR #22](https://github.com/techrote/sandimations/pull/22) · [owner queue](https://github.com/techrote/scheduled-strike-teams/issues/9) |
| Quick editorial | flatCAD | Owner review of Beta 1 docs-only PR | [PR #32](https://github.com/techrote/flatCAD/pull/32) |
| Manual hardware | HWiNFOterm | Live HWiNFO + Windows Terminal acceptance | [PR #1](https://github.com/techrote/HWiNFOterm/pull/1) |
| Manual runtime | INTUIT3D | Windows wrong-body/valid-cut evaluation | [PR #351](https://github.com/techrote/INTUIT3D/pull/351) |

## Review log

- **2026-11-13 — Setup.** Campaign repository initialized, seven potential teams and owner gate documented. No campaign worker started. First real orchestration update must refresh the task inventory and annotate each team's actual worker ID and source SHA.
- **2026-11-13 — Flexdiffusion launch.** Created and verified three active hourly workers for independent PR #9, upstream sampler PR #8 and dependent workspace PR #10. IDs preserved in [TEAM-06 #7](https://github.com/techrote/scheduled-strike-teams/issues/7). Capacity 4/10 including prior ShadeDoomVK monitor. The initial 48-run schedules are short-lived; pause/rotate early on completion or owner gate.
- **Next review:** update this board only after inspecting team issue receipts and target repo evidence. The separate campaign issue is the live audit trail; do not erase previous dated milestones.

## Board update rules

Make small, dated changes. Never mark a team ACTIVE without its actual enabled automation ID(s), READY_OWNER without exact SHA/CI/acceptance evidence, or COMPLETE merely because a PR is marked mergeable. Keep owner approval and release state explicit. Retire old workers promptly; do not recycle team issue identity for unrelated projects without documenting the change.
