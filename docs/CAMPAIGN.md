# Campaign plan — 13–27 November 2026

**Owner decision status:** the campaign is authorised. **Flexdiffusion's three hourly workers were explicitly approved and activated on 13 November; the other team allocations remain proposals.** [Campaign issue #1](https://github.com/techrote/scheduled-strike-teams/issues/1) holds live decisions.

## Outcome and measurement

Bring the greatest practical number of distinct projects to a source-verified, **owner-review-ready** scoped state. Do not optimise for generated commits, test reruns, tickets closed without evidence, or schedules kept busy.

Report separately:

1. **Release/project-ready** — product's agreed release/evaluation scope passes all accessible technical gates; only owner review/acceptance remains.
2. **PR/tranche-ready** — a bounded change is source-exact and tested; broader project work may remain.
3. **Owner-action blocked** — named physical, administrative, editorial or credential action prevents further progress.
4. **Technical HOLD** — an unresolved defect, incompatible integration or unqualified test exists.
5. **Deferred/retired** — no useful next hourly run until circumstances change.

Count each repository **once** in the distinct-project metric; count PR/issue dispositions separately. A draft PR that is mergeable is not automatically ready. A CI-green host build is not a native-hardware pass. Close or merge target issues/PRs only after owner authorization and verified compliance with target project policy.

## Resource envelope

- **10 enabled hourly task slots maximum, globally**, inclusive of existing non-campaign schedules; recheck real status before every activation.
- **1–6 workers per strike team**; initial use generally 1–2. Add workers only to separately owned paths or independent reviews.
- **1–5 owner-triggered GPT-6 Pro sessions** per complex engagement when justified, for kickoff, difficult debugging, reconciliation and final review. Pro is not a permanent scheduled shepherd.
- Owner review cadence: typically morning, midday and evening, at minimum daily. There is no expectation of 24/7 attendance by the owner.
- No scheduled team should be assumed to last all 14 days. On success or human-only blockade, stop recurring edits and free its slot promptly.

### Original allocation proposal (historical baseline)

**Superseded in part:** Flexdiffusion is now assigned **3 active workers** rather than the original one. The table below records the original portfolio proposal; **do not activate all remaining proposed workers on top of the three new workers**. At the last verified check, 4/10 tasks were enabled (Flexdiffusion ×3, ShadeDoomVK ×1), leaving 6 slots. See the [current board](../status/BOARD.md).

The initial audit of task schedules found 1 enabled existing ShadeDoomVK CI A/B monitor and 9 available capacity slots. This is a **point-in-time observation**, not a guarantee of the current active count.

| Team | Proposed slots | Target | Coordination |
| --- | ---: | --- | --- |
| Greygen | 2 | Real Pages-path smoke #46 + PWA icons #47, release audit #45 | [#2](https://github.com/techrote/scheduled-strike-teams/issues/2) |
| HWiNFOterm | 1 | Existing reliability PR #1 | [#3](https://github.com/techrote/scheduled-strike-teams/issues/3) |
| INTUIT3D | 1 | Wrong-body cut correctness PR #351 | [#4](https://github.com/techrote/scheduled-strike-teams/issues/4) |
| Steelmoth | 2 | Packaging/CI PRs and oracle dependency chain | [#5](https://github.com/techrote/scheduled-strike-teams/issues/5) |
| DashMinimix | 1 | Existing source-switch PR #18 first | [#6](https://github.com/techrote/scheduled-strike-teams/issues/6) |
| Flexdiffusion | 1 | PNG alpha-mask PR #9 first | [#7](https://github.com/techrote/scheduled-strike-teams/issues/7) |
| Omnipanel | 1 | Publication PR #90, then resource dashboard #72 | [#8](https://github.com/techrote/scheduled-strike-teams/issues/8) |
| Existing ShadeDoomVK CI monitor | 1 | Finish A/B monitoring; retire when evidence delivered | Not a new campaign team |
| **Total proposed** | **10** | **9 potential new workers + 1 existing monitor** | **None newly enabled by this plan** |

**Fast-track human unlock:** [sandimations PR #22](https://github.com/techrote/sandimations/pull/22) reports near-complete qualification but missing Pages admin configuration; see [owner gates #9](https://github.com/techrote/scheduled-strike-teams/issues/9). When enabled, insert a one-worker finisher into the first released slot. [flatCAD #32](https://github.com/techrote/flatCAD/pull/32) is principally an owner editorial review rather than an ongoing hourly task.

### Why this selection

The portfolio mixes short, reviewable existing PRs (HWiNFOterm, INTUIT3D, Flexdiffusion, Omnipanel) with two small independent improvements in Greygen, cross-PR hardening in Steelmoth, and a bounded review of DashMinimix's existing candidate. These compete better on likelihood of review-ready handoff than large unfinished research programmes with dependent physical gates.

## Rotation windows — flexible, not fixed contracts

| Window | Main objective | Rotation rule |
| --- | --- | --- |
| 13–15 Nov | Launch and validate existing candidates; expose owner gates | Free slot after first source-exact handoff |
| 15–18 Nov | Finish small projects; collect qualified issue/PR dispositions | Sandimations first after Pages unlock; use freed slots on Omnipanel #72 / DashMinimix / remaining Greygen |
| 18–22 Nov | Specialist technical convergence | Consider ASCIIomium (up to 2), Fixitup (1–2), or OrcaSlicer #27 only if predecessors/CI are ready |
| 22–26 Nov | Final source-matched qualification and release packages | Do not initiate substantial new features without credible same-window exit |
| 27 Nov | Campaign reconciliation, stop schedules, prepare owner-review digest | Record READY / owner action / technical HOLD / deferred for every lane |

**Proposed campaign target:** 5–6 distinct review-ready scoped projects; 8+ is a stretch target, not a prediction.

## Decision algorithm for each manual review

1. **Refresh:** list enabled scheduled tasks and exact ownership; never infer availability from planned allocations.
2. **Verify:** read last material result, GitHub PR/issue state, current head, source-matched CI and any source changes since qualification.
3. **Classify:** ready-owner, still progressing, human-only blocked, technical hold, repeated no-progress, or superseded.
4. **Intervene:** request physical/admin action, invoke Pro once for a hard problem, or freeze competing overlapping writers.
5. **Rotate:** disable completed or blocked schedules and enable the highest-priority ready replacement, preserving the 10-slot cap. Always log actual schedule IDs.
6. **Record:** post a dated campaign update on [#1](https://github.com/techrote/scheduled-strike-teams/issues/1), a specific issue comment on the relevant team issue, and periodically update [status/BOARD.md](../status/BOARD.md) as the dated snapshot.

Two hourly executions without meaningful progress trigger Pro assessment. Repeated identical CI failures must not spawn indefinite retries. Around 24–36 hours of unresolved engagement triggers an allocation review; three consecutive manual reviews without a credible path justify pausing. These are decision heuristics, not reasons to abort a nearly completed fix.

## Candidate expansion queue

| Next project | Appropriate trigger | Primary risk |
| --- | --- | --- |
| sandimations | Owner enabled Pages; one freed slot | Deployment/admin gate |
| ASCIIomium | Two workers available, Windows/CEF proof achievable | Native runtime qualification |
| Fixitup | Cross-repo permissions and scope boundaries agreed | Admin/security authorization |
| OrcaSlicer-PlanePath-fork | PR #27 and dependent conflict tree verified | Large native slicer CI |
| Relay-Moth-Forest | PERF-004 predecessor objectively admitted | Performance regression dependency |
| flatCAD | Owner requests fixes from PR #32 review | Editorial, not engineering throughput |
| ohmy | Pro identifies unambiguous winning integration head | Overlapping existing draft PRs |
| k80nsai | Native K80/CUDA test access or CPU-only target selected | Hardware/driver gate |

No team is permanently entitled to its slot. Deprioritise long-running CyberSand, radiCADSAC, ZaagGenZ, neurounner, ezvm, complex hardware experiments and externally gated research unless a very specific high-value, short review-ready task emerges.

## Owner safety and completion

- No auto-merges, release publication, deployment policy changes, secrets exposure, irreversible cleanups, or target-repository issue closure without separate explicit approval.
- Respect all target-repository AGENTS.md and engineering instructions, including their narrower acceptance policies.
- Preserve Draft/HOLD until owner acceptance; never call a project ready from a single stale CI pass.
- Campaign documents are guides; real status is source-linked to target GitHub and schedule IDs. Record ambiguities rather than guessing.
- On 27 Nov publish a closing digest and pause campaign tasks; do not silently keep them running.
