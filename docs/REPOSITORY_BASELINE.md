# Repository assessment baseline — 13 November 2026

**Scope:** 109 repositories returned for techrote at inventory time, assessed by oldest last code push first, then real open issue/PR content, branch/CI dependencies and likelihood of source-verified owner handoff. The counts and activity dates below are **point-in-time**, not live truth.

## Findings

- The least recently pushed repos (late August/early September) are mostly small prototypes without outstanding issues/PRs: EdgeCraft, Brachistochrone-Lab, CyberTerm, PNG2ANSI, PlasmaTerm, pyANSI, ThermoPipeParameter, buildtest and XenoField. They may merit release polish but not backlog-closure workers.
- Large numbers of issues in September projects are often dependency-ordered design plans, not independently closable defects. Examples: 6700 hardware/host qualification, terman WPF product build, ESPtelepathy physical experiments, slop-commander cross-component integration.
- A **small already-implemented PR with an independently testable gate** is generally the fastest path to a review-ready scope.
- Multiple overlapping draft PRs may need careful consolidation rather than independent merging. False closures and re-audits reduce campaign value.
- Actual native hardware, GPU, Windows Terminal, GitHub administration and public deployment require their own evidence. CI success is not a substitute.

## Candidate portfolio (last pushed, open issue / PR counts at assessment)

| Repository | Last pushed | Issues / PRs | First useful action | Coordination |
| --- | --- | ---: | --- | --- |
| [DashMinimix](https://github.com/techrote/DashMinimix) | 12 Sep | 9 / 1 | [PR #18](https://github.com/techrote/DashMinimix/pull/18) config preservation then bounded audits | [team #6](https://github.com/techrote/scheduled-strike-teams/issues/6) |
| [sandimations](https://github.com/techrote/sandimations) | 16 Sep | 2 / 1 | [PR #22](https://github.com/techrote/sandimations/pull/22), enable Pages then public deployment | [owner gates #9](https://github.com/techrote/scheduled-strike-teams/issues/9) |
| [Omnipanel](https://github.com/techrote/omnipanel) | 19 Sep | 50 / 2 | [PR #90](https://github.com/techrote/omnipanel/pull/90) publication, then [#72](https://github.com/techrote/omnipanel/pull/72) dashboard | [team #8](https://github.com/techrote/scheduled-strike-teams/issues/8) |
| [Fixitup](https://github.com/techrote/fixitup) | 24 Sep | 11 / 0 | [FUP-001](https://github.com/techrote/fixitup/issues/1) auditor before cross-repo repairs | Expansion queue |
| [k80nsai](https://github.com/techrote/k80nsai) | 26 Sep | 21 / 2 | [PR #27](https://github.com/techrote/k80nsai/pull/27) host oracle; CUDA/K80 physical gate separate | Expansion queue |
| [Greygen](https://github.com/techrote/greygen) | 7 Oct | 5 / 0 | [#46](https://github.com/techrote/greygen/issues/46) Pages-path browser test, [#47](https://github.com/techrote/greygen/issues/47) icons | [team #2](https://github.com/techrote/scheduled-strike-teams/issues/2) |
| [OrcaSlicer-PlanePath-fork](https://github.com/techrote/OrcaSlicer-PlanePath-fork) | 14 Oct | 14 / 3 | [PR #27](https://github.com/techrote/OrcaSlicer-PlanePath-fork/pull/27) small fix with conflicts; #22 Lua larger | Expansion queue |
| [Flexdiffusion](https://github.com/techrote/flexdiffusion) | 1 Nov | 0 / 4 | [PR #9](https://github.com/techrote/flexdiffusion/pull/9); #10 stacked on #8 | [team #7](https://github.com/techrote/scheduled-strike-teams/issues/7) |
| [ASCIIomium](https://github.com/techrote/ASCIIomium) | 3 Nov | 15 / 5 | [PRs #40–44](https://github.com/techrote/ASCIIomium/pulls) with Windows/CEF native gate | Expansion queue |
| [Relay-Moth-Forest](https://github.com/techrote/Relay-Moth-Forest) | 3 Nov | 1 / 1 | [PR #39](https://github.com/techrote/Relay-Moth-Forest/pull/39), dependent PERF-004 | Expansion queue |
| [HWiNFOterm](https://github.com/techrote/HWiNFOterm) | 4 Nov | 0 / 1 | [PR #1](https://github.com/techrote/HWiNFOterm/pull/1), telemetry/terminal reliability | [team #3](https://github.com/techrote/scheduled-strike-teams/issues/3) |
| [Steelmoth](https://github.com/techrote/steelmoth) | 6 Nov | 5 / 8 | PR #121/#124 and #119/#120/#125 consolidation | [team #5](https://github.com/techrote/scheduled-strike-teams/issues/5) |
| [flatCAD](https://github.com/techrote/flatCAD) | 9 Nov | 9 / 3 | [PR #32](https://github.com/techrote/flatCAD/pull/32) Beta 1 docs owner review | [owner gates #9](https://github.com/techrote/scheduled-strike-teams/issues/9) |
| [INTUIT3D](https://github.com/techrote/INTUIT3D) | 9 Nov | 1 / 3 | [PR #351](https://github.com/techrote/INTUIT3D/pull/351), wrong-body semantic refusal | [team #4](https://github.com/techrote/scheduled-strike-teams/issues/4) |

Other significant repos, **not initial cleanup targets**: [CyberSand](https://github.com/techrote/cybersand), [ShadeDoomVK](https://github.com/techrote/ShadeDoomVK), [ZaagGenZ](https://github.com/techrote/zaaggenz), [radiCADSAC](https://github.com/techrote/radiCADSAC), [MachineHumanAudioCybersemiotics](https://github.com/techrote/MachineHumanAudioCybersemiotics), [neurounner](https://github.com/techrote/neurounner), [ezvm](https://github.com/techrote/ezvm), [ohmy](https://github.com/techrote/ohmy) and [terman](https://github.com/techrote/terman). Reasons include ongoing concurrent development, research rigor, overlapping PRs, substantial new implementation or native/owner dependencies.

## Evidence nuances and readiness pitfalls

- **sandimations #22:** historical PR text reports fully green final-head code/Pages-base smoke, but a 403 on GitHub Pages site creation. Administrator enablement plus live deployment verification remains required.
- **HWiNFOterm #1:** candidate reports 90/95 Linux tests passing and five Windows-only skipped locally; hosted and physical Windows evidence must be refreshed.
- **INTUIT3D #351:** semantic runtime correction is narrowly scoped; it is not general OCCT/STEP acceptance.
- **flatCAD #32:** docs-only; user editorial assessment, not another broad engineering programme.
- **Greygen #45:** original audit expressly says its earlier CI references are stale relative to audited main. Fresh exact-head checks required.
- **Omnipanel #90:** publication fix explicitly does **not** implement Codex master [issue #89](https://github.com/techrote/omnipanel/issues/89). Do not close #89.
- **Steelmoth #119/#120/#125:** dependent oracle branches; separate integration and independent review. Do not declare physical GTX 1650S or final WebGPU promotion.
- **DashMinimix #18:** HWiNFO source-switch preservation is a targeted change; custom persisted Qt dashboard problem belongs in #9.
- **Flexdiffusion #10:** stacked on #8, not an independent same-base merge candidate.

## Refresh rule

Before selecting a new team, check current main SHA, PR status, issue text/owner constraints, last significant CI run and existing scheduled workers. The purpose of this document is to preserve **why** a candidate was selected, not to serve as a live GitHub mirror.
