# Campaign status board — snapshot

**Snapshot time:** 14 November 2026, after TRIO-017 software qualification and live schedule inspection (~10:00 GMT).  
**Authoritative live coordination:** [campaign #1](https://github.com/techrote/scheduled-strike-teams/issues/1) and the linked team issues.  
**All three Flexdiffusion workers (A/B/C) completed bounded PR-level scopes, posted evidence-backed handoffs and self-paused.** See [TEAM-06 #7](https://github.com/techrote/scheduled-strike-teams/issues/7).

## Capacity and health

| Indicator | Last recorded | Evidence/status |
| --- | --- | --- |
| Maximum hourly slots | 10 | Owner-set global campaign cap |
| Enabled tasks at latest audit | **13 global, 0 strike-team** | 7 SANDMAPS + 6 CyberSand schedules currently enabled; prior Flexdiffusion/CI monitors paused |
| Additional campaign slots under original total-10 ceiling | **0 until owner reallocation** | Global enabled count is 13, above the campaign's stated 10 total limit; do not activate new tasks automatically |
| Eligible unstarted candidate allocation | **6 proposed slots** | Greygen 2, HWiNFOterm 1, INTUIT3D 1, Steelmoth 2; only start after explicit approval and fresh slot audit |
| Active campaign worker IDs | **0** | A: `6af74cbd1a788191be877e450ca62333`, B: `6af74cbef05c8191b3cf5686b18d0858`, C: `6af74cc186bc8191aec39f3f19f65bad` **all paused** |
| Verified scoped READY_OWNER transitions | **1 software release candidate + 3 PR tranches** | tuisynth-codex v0.1.0 PR #35: exact-head 4/4 CI PASS, owner hardware acceptance pending; Flexdiffusion #8/#9/#10 remain PR-level handoffs |
| Human gates | sandimations Pages, flatCAD editorial, Windows acceptance | [owner queue #9](https://github.com/techrote/scheduled-strike-teams/issues/9) |

## Team lanes

| Rank | Team issue | Proposed worker slots | State | Current first target | Exact-head qualification / next milestone |
| ---: | --- | ---: | --- | --- | --- |
| 1 | [Greygen #2](https://github.com/techrote/scheduled-strike-teams/issues/2) | 2 | **CANDIDATE** | [greygen #46](https://github.com/techrote/greygen/issues/46), [#47](https://github.com/techrote/greygen/issues/47) | Actual Pages-path browser CI and icon/install matrix |
| 2 | [HWiNFOterm #3](https://github.com/techrote/scheduled-strike-teams/issues/3) | 1 | **CANDIDATE** | [PR #1](https://github.com/techrote/HWiNFOterm/pull/1) | Exact-head Windows/Linux CI, explicit physical acceptance |
| 3 | [INTUIT3D #4](https://github.com/techrote/scheduled-strike-teams/issues/4) | 1 | **CANDIDATE** | [PR #351](https://github.com/techrote/INTUIT3D/pull/351) | Wrong-body cut semantics, Ubuntu+Windows CI |
| 4 | [Steelmoth #5](https://github.com/techrote/scheduled-strike-teams/issues/5) | 2 | **CANDIDATE** | [PR #121](https://github.com/techrote/steelmoth/pull/121), [#124](https://github.com/techrote/steelmoth/pull/124), [#119](https://github.com/techrote/steelmoth/pull/119) | Independent review, dependency-order reconcile |
| 6 | [Flexdiffusion #7](https://github.com/techrote/scheduled-strike-teams/issues/7) | **3 completed / 0 enabled** | **A/B/C READY_OWNER / merge HOLD** | [PR #9](https://github.com/techrote/flexdiffusion/pull/9), [#8](https://github.com/techrote/flexdiffusion/pull/8), [#10](https://github.com/techrote/flexdiffusion/pull/10) | A: inpainting; B: sampler; C: Blend Lab. Each 48 hourly runs, owner-gated handoff |
| — | [tuisynth-codex #10](https://github.com/techrote/scheduled-strike-teams/issues/10) | **0 scheduled / 1 manual Pro** | **READY_OWNER, software-qualified** | [TRIO-017 PR #35](https://github.com/techrote/tuisynth-codex/pull/35) | Exact SHA `40584a81...`, 4/4 hosted lanes PASS; 10 artifacts retained; owner audio/MIDI/Windows Terminal validation and merge approval pending |
| — | Existing ShadeDoomVK monitor | 1 | **PAUSED AT LATEST AUDIT** | CI A/B results | Paused independently of Worker C; not counted as enabled |

**Capacity last verified: 13 globally enabled, 0 strike-team schedules, no new slots available under the original total-10 ceiling without owner reallocation.** This is a live observation, not a request to pause unrelated SANDMAPS/CyberSand work. The enabled automation list is the source of truth.

## Retired or reference-only team proposals

| Repository | Coordination | Disposition |
| --- | --- | --- |
| [DashMinimix](https://github.com/techrote/DashMinimix) | [Retired team #6](https://github.com/techrote/scheduled-strike-teams/issues/6) | Abandoned; **HWiNFOterm is the fresh replacement**. No workers or PR/issue closure campaign. |
| [Omnipanel](https://github.com/techrote/omnipanel) | [Dormant team #8](https://github.com/techrote/scheduled-strike-teams/issues/8) | Near-abandoned; potential philosophical/intent reference only, not an engineering queue. |

## Recently completed manual Pro engagement

- **tuisynth-codex TRIO-017:** one sustained Pro engagement produced the software-qualified v0.1.0 candidate in [Draft PR #35](https://github.com/techrote/tuisynth-codex/pull/35), held for owner review. Source `40584a81a42b86ea4cfd87e2277b16036c373bcb`; [CI #43548630964](https://github.com/techrote/tuisynth-codex/actions/runs/43548630964) 4/4 jobs SUCCESS; 10 artifacts present, expiring 14 December 2026. Separate physical audio/MIDI/Windows Terminal and distribution/merge gates still outstanding. [Acceptance tracker #10](https://github.com/techrote/scheduled-strike-teams/issues/10).

## Owner action / zero-worker lanes

| Priority | Project | Action | Link |
| --- | --- | --- | --- |
| Urgent unblock | sandimations | Enable GitHub Pages if missing; then one worker can finish live deploy | [PR #22](https://github.com/techrote/sandimations/pull/22) · [owner queue](https://github.com/techrote/scheduled-strike-teams/issues/9) |
| Quick editorial | flatCAD | Owner review of Beta 1 docs-only PR | [PR #32](https://github.com/techrote/flatCAD/pull/32) |
| Manual hardware | HWiNFOterm | Live HWiNFO + Windows Terminal acceptance | [PR #1](https://github.com/techrote/HWiNFOterm/pull/1) |
| Manual runtime | INTUIT3D | Windows wrong-body/valid-cut evaluation | [PR #351](https://github.com/techrote/INTUIT3D/pull/351) |
| Manual product | tuisynth-codex | Download Windows/Python 3.11 candidate, checksum, run AURORA/LOOM/DRIFT audio/MIDI/terminal/10-minute checks; decide licence/merge/release separately | [PR #35](https://github.com/techrote/tuisynth-codex/pull/35) · [team #10](https://github.com/techrote/scheduled-strike-teams/issues/10) |

## Review log

- **2026-11-13 — Setup.** Campaign repository initialized, seven potential teams and owner gate documented. No campaign worker started. First real orchestration update must refresh the task inventory and annotate each team's actual worker ID and source SHA.
- **2026-11-13 — Flexdiffusion launch.** Created and verified three active hourly workers for independent PR #9, upstream sampler PR #8 and dependent workspace PR #10. IDs preserved in [TEAM-06 #7](https://github.com/techrote/scheduled-strike-teams/issues/7). Capacity 4/10 including prior ShadeDoomVK monitor. The initial 48-run schedules are short-lived; pause/rotate early on completion or owner gate.
- **2026-11-13 — Flexdiffusion Worker C handoff/rotation.** PR #10 at `f789dc7fdddbfeb99e88fb72d814385a8764ace0` has source-exact push and PR CI PASS, including real Chromium blend and request-isolation checks; hold merge for upstream PR #8/#2, PR #9 reconciliation and Windows/Firefox model acceptance. Worker C automation paused. Latest inventory: only Flexdiffusion A/B enabled (2/10), and ShadeDoomVK no longer enabled.
- **2026-11-13 — Owner portfolio correction.** DashMinimix removed from active candidate allocation because HWiNFOterm is its replacement; Omnipanel withdrawn from active implementation planning and retained as philosophical/architectural intent reference. Historical coordination issues #6/#8 marked RETIRED/DORMANT; neither had active workers. No schedules added, no source PRs changed. Candidate proposal now focuses on Greygen, HWiNFOterm, INTUIT3D and Steelmoth, in addition to active Flexdiffusion.
- **2026-11-13 — Flexdiffusion Worker A handoff/rotation.** PR #9 at `88aadfa72f41737ba1d43d97ed82f2b01bf4c574` passed exact-head push + synthetic PR checks (15/15 Node tests, 29 Chrome assertions). Windows 11 Firefox actual inpainting generation remains owner acceptance; merge held. A self-paused; C already paused; B alone enabled (1/10). See [A handoff](https://github.com/techrote/scheduled-strike-teams/issues/7#issuecomment-6862629563) and [C handoff](https://github.com/techrote/scheduled-strike-teams/issues/7#issuecomment-6862304064).
- **2026-11-13 — Flexdiffusion Worker B handoff and Top 20 refresh.** PR #8 at `70be959a9a1f9aab5250229a438738cb9617ff24` passes source-exact Ubuntu and Windows native CPU solver/model-free HTTP suites **27/27 per OS with no skips**; remains Draft/HOLD for upstream PR #2 and actual Windows/Firefox/SD1.x GPU acceptance. B self-paused. All three team schedules paused (0/10 active). See [B handoff](https://github.com/techrote/scheduled-strike-teams/issues/7#issuecomment-6863530061). [Ranked Top 20](../docs/TOP20_RECOMMENDATIONS.md) supersedes old team proposals for selection, but does not authorise activation.
- **2026-11-14 — TRIO-017 one-Pro successful finisher.** [PR #35](https://github.com/techrote/tuisynth-codex/pull/35) holds one reproducible v0.1.0 software candidate at `40584a81...` with all four CI jobs passing on the exact source and 10 nonexpired artifacts. New [tracking issue #10](https://github.com/techrote/scheduled-strike-teams/issues/10) records specific owner audio/MIDI/Windows Terminal and release gates; count as one software candidate review-ready, not an accepted release. Live enabled schedule inventory now has 13 non-strike-team tasks, exceeding the original total-10 campaign cap; no schedules changed.
- **Next review:** update this board only after inspecting team issue receipts and target repo evidence. The separate campaign issue is the live audit trail; do not erase previous dated milestones.

## Board update rules

Make small, dated changes. Never mark a team ACTIVE without its actual enabled automation ID(s), READY_OWNER without exact SHA/CI/acceptance evidence, or COMPLETE merely because a PR is marked mergeable. Keep owner approval and release state explicit. Retire old workers promptly; do not recycle team issue identity for unrelated projects without documenting the change.
