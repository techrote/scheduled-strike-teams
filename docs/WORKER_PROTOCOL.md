# Strike-team protocol

This document is the reusable contract for any scheduled worker or manually triggered GPT-6 Pro consultant in the 13–27 November 2026 campaign.

## Preflight: every engagement

1. Read [campaign #1](https://github.com/techrote/scheduled-strike-teams/issues/1), [plan](CAMPAIGN.md), [board](../status/BOARD.md) and **your own team issue**.
2. Read the target repository's current main, AGENTS.md, authoritative issue/PR description, latest reviews, CI and ongoing work. Historical SHAs in this hub are checkpoints, not proof of present head.
3. Refresh enabled schedule allocation and check for competing work. Do not start a conflicting writer or an unapproved new team.
4. Adopt one **precisely bounded target**, branch, file ownership and acceptance contract; prefer improving an existing PR to opening another.
5. Keep decisions and evidence in the team issue; the target issue/PR remains the technical specification. Do not place live mutable status exclusively in this document.

## Working rules

- Complete the existing scoped feature: code, tests, CI, native or browser checks where actually available, defect repair and evidence. Do not stop at architecture analysis or scaffolding.
- Where a defect is confirmed, demonstrate a failing-before regression and passing-after regression when reasonably possible.
- Keep changes focused. Do not introduce new settings, architectures, monitoring frameworks, or 'audit infrastructure' unless required by acceptance.
- If other specialists are assigned, maintain explicit nonoverlapping branches/paths; never overwrite another specialist's head. Obtain a reconciliation owner before integrating.
- Use fresh exact-head GitHub Actions evidence; distinguish source-hash, tree-hash and synthetic merge checks. Stale green runs do not qualify a changed head.
- Treat CI signals as scoped. Windows, browser, GPU, physical devices, security settings and production deployment require their corresponding real validation; report unsupported gates plainly.
- No direct merges, issue closures, public releases, credentials or permission changes, destructive actions, or target security-policy changes without separate owner authorization.
- Keep long-running test jobs and runs bounded. Stop/release resources upon cancellation or completion.
- Escalate reproducible architectural conflicts or two nonproductive hourly cycles to GPT-6 Pro/owner instead of looping indefinitely.

## Hourly receipt — append to your team issue only if materially different

**Date/time UTC:**  
**State:** CANDIDATE / ACTIVE / READY_OWNER / OWNER_ACTION / HOLD / RETIRED  
**Schedule ID / role / owned branch:**  
**Target and latest head SHA:**  
**Changed since last run:**  
**Verified evidence:** commands, test counts, OS/browser, GitHub Actions URL and commit match; include negative-control results where relevant  
**Outstanding blockers:** precise requirement, owner gate or failing assertion  
**Next bounded action:** one concrete step  
**Pause/rotate recommendation:** continue / escalate / stop

Do not pad with repeated summaries, invent times or claim background work was done. For an already completed target, emit a terminal receipt and stop editing.

## READY_OWNER handoff dossier

A scoped deliverable may be called **READY_OWNER** only when the following are provided:

- Exact repository, target issue/PR, target base, candidate head SHA and changed-file scope.
- Brief behavioral summary and compatibility/rollback assessment.
- All required automated regressions, source-exact CI runs and interpretation of skips.
- Native/graphical/browser evidence where available; unsupported hardware/user-only checks separately named.
- Merge-order/dependency/conflict status and independent review finding.
- A small, reproducible owner acceptance procedure, preferably single-paste on Windows where relevant.
- Explicit **GO/HOLD** recommendation, residual risks and action owner.
- Whether this is a complete release/evaluation candidate or only one PR/tranche.

If any required accessible technical gate fails, mark HOLD; if only an external administrative/physical step can unlock further checks, mark OWNER_ACTION. Only the owner approves merge/release and decides when the overall project is accepted.

## Orchestration and conflict rules

- One central [campaign issue #1](https://github.com/techrote/scheduled-strike-teams/issues/1) for slot and priority decisions.
- One team issue per engagement, not one issue per worker execution.
- One [owner gates issue #9](https://github.com/techrote/scheduled-strike-teams/issues/9) for short human interventions.
- A dated [board](../status/BOARD.md) is a snapshot, not a continuously accurate register. Recheck before spending capacity.
- If real activity diverges from any plan, record actual schedule IDs and refresh docs; do not retrofit history.
- Manual GPT-6 Pro work should diagnose, integrate or adjudicate. It should not compete with an active writer on the same branch.
