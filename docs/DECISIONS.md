# Campaign decision log

Each entry should distinguish an **approved owner decision** from a **proposal or observation**. Do not treat a drafted allocation as permission to activate tasks. Record later changes append-only with dated rationale and links to [campaign #1](https://github.com/techrote/scheduled-strike-teams/issues/1).

## 2026-11-13 — Established by owner

- **Approved:** A bounded 14-day repository strike-team effort, aiming for the greatest number of projects brought to the ready-after-human-review stage.
- **Approved:** Up to **10 total concurrently enabled hourly scheduled tasks**, not 10 per project; teams of approximately 1–6 specialists, with temporary allocation and reassignment.
- **Approved:** Owner expects to review progress at least daily, often about three times each day, and may intervene manually for acceptances and operational blockers.
- **Approved:** Manually triggered GPT-6 Pro engagements are a first-class resource for kickoff, troubleshooting, complex assessment and reconciliation, not an always-on substitute for progress.
- **Approved:** [scheduled-strike-teams](https://github.com/techrote/scheduled-strike-teams) is the permanent campaign orchestration, progress and reference repository.
- **Guardrail retained:** Target changes, test results and reviews must remain in the target repository; do not make this hub an alternative feature specification or accept unreviewed merges.

## 2026-11-13 — Initial analysis, not an approval to start

- **Proposed:** A nine-worker initial allocation: Greygen 2, HWiNFOterm 1, INTUIT3D 1, Steelmoth 2, DashMinimix 1, Flexdiffusion 1, Omnipanel 1. Combined with the one existing ShadeDoomVK CI A/B monitor this would reach the ceiling of 10.
- **Observed at initial schedule inspection:** One enabled schedule (ShadeDoomVK CI A/B monitor); other listed campaign/legacy schedules paused. This is a timestamped observation, not a continuously verified count.
- **Proposed:** Prioritise sandimations as the first one-slot fast-track replacement once the repository Pages administrative gate is cleared.
- **Proposed:** FlatCAD #32 as an owner-editorial quick win without a new hourly worker.
- **Proposed targets:** 5–6 distinct scoped review-ready projects by 27 Nov; 8+ stretch. These are planning targets, not forecasts or achieved results.
- **Not done:** No campaign schedules started or retuned; no target-repository PRs merged, issues closed, or settings changed during hub setup.

## 2026-11-13 ~17:45 UTC — Approved and executed: Flexdiffusion three-worker strike team

- **Approved:** User explicitly requested three scheduled workers for Flexdiffusion.
- **Executed:** Three enabled hourly automations with 48 recurrences each:
  - Inpainting PR #9: `6af74cbd1a788191be877e450ca62333`
  - Sampler PR #8: `6af74cbef05c8191b3cf5686b18d0858`
  - Blend Lab PR #10: `6af74cc186bc8191aec39f3f19f65bad`
- **Verified:** 4 enabled tasks including the existing ShadeDoomVK A/B monitor, leaving 6 of the campaign's 10 slots free at launch.
- **Ownership:** Three separate PR branches; #8 depends on #2, #10 depends on #8 and #9 stands alone on main. Shared-file reconciliations require owner/Pro review.
- **Tracking:** [TEAM-06 #7](https://github.com/techrote/scheduled-strike-teams/issues/7); [campaign #1](https://github.com/techrote/scheduled-strike-teams/issues/1).
- **Previous allocation:** The original 1-slot Flexdiffusion allocation is superseded. Do not instantiate all remaining initial proposals without rechecking the ten-task cap.
- **Human gate:** Merge/release/issue closure still require explicit owner approval; these schedules may be paused early on READY_OWNER or OWNER_ACTION.

## 2026-11-13 ~19:14 UTC — Owner correction: DashMinimix superseded; Omnipanel dormant

- **Approved owner disposition:** DashMinimix is an abandoned predecessor project. **HWiNFOterm is the fresh successor implementation** of the original telemetry concept, developed with significantly more accumulated experience. The current HWiNFOterm architecture, code, PRs and acceptance obligations are authoritative. Do not automatically transplant DashMinimix features/code or schedule its stale issue/PR backlog.
- **Approved owner disposition:** Omnipanel is near-abandoned as a product. It may remain useful as a **philosophical and design-intent communication reference** for future projects, subject to owner choice, but not as an active engineering campaign.
- **Allocation consequence:** Withdraw DashMinimix's original 1-slot proposal and Omnipanel's original 1-slot proposal. **Neither ever had an activated worker** in this campaign, so this releases proposed capacity only, not two actually enabled schedules. No replacement workers created by this update.
- **Historical preservation:** [DashMinimix coordination #6](https://github.com/techrote/scheduled-strike-teams/issues/6) marked RETIRED, [Omnipanel coordination #8](https://github.com/techrote/scheduled-strike-teams/issues/8) marked DORMANT; original notes remain for provenance. [HWiNFOterm #3](https://github.com/techrote/scheduled-strike-teams/issues/3) is the active successor candidate.
- **Planning effect:** The eligible unstarted candidate teams are Greygen, HWiNFOterm, INTUIT3D and Steelmoth. Existing Flexdiffusion scheduled work continues separately under its explicit approval. Recheck active schedule count at every allocation.
- **Source repositories unchanged:** Neither target repository was archived, modified, had issues/PRs closed, or acquired an automation through this disposition.

## Future decision format

### YYYY-MM-DD HH:MM UTC — [approved / proposed / observed]

- **Change:**
- **Why:** current, source-exact evidence and comparative value
- **Impacted schedules/IDs:**
- **Project/team issues:**
- **Owner confirmation or approval:**
- **Rollback/reallocation decision:**
