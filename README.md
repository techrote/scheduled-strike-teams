# Scheduled Strike Teams

**Campaign:** 13–27 November 2026 · **Owner:** techrote · **State:** active — see [current board](status/BOARD.md) for enabled count

This repository is the coordination and evidence hub for short-lived hourly engineering strike teams working across the techrote repositories. Its purpose is to bring the maximum practical number of **distinct projects to verified owner-review readiness** within a fourteen-day campaign, not to maximise commits, run counts, or issue closures.

## Start here

- [Campaign plan](docs/CAMPAIGN.md) — priorities, proposed allocations, rotation rules and owner interventions.
- [Campaign board](status/BOARD.md) — dated snapshot of team lanes, evidence and open gates.
- [Worker protocol](docs/WORKER_PROTOCOL.md) — scope ownership, source-verification and reporting contract.
- [Ready-to-use prompts](docs/PROMPTS.md) — hourly specialist, GPT-6 Pro and owner review templates.
- [Repository assessment](docs/REPOSITORY_BASELINE.md) — evidence-linked starting candidates and alternative queue.
- [Decision log](docs/DECISIONS.md) — approved decisions versus proposals.
- [Campaign issue #1](https://github.com/techrote/scheduled-strike-teams/issues/1) — live orchestration and allocation decisions.
- [Owner gates #9](https://github.com/techrote/scheduled-strike-teams/issues/9) — administrator, editorial and physical acceptance actions.
- [Team issues #2–8](https://github.com/techrote/scheduled-strike-teams/issues) — specialist progress receipts and handoffs.

## Teams summary

| Repo | Ideal workers | Last assigned workers | Estimated work remaining | Last significant milestone achieved |
| --- | ---: | ---: | --- | --- |
| [Greygen](https://github.com/techrote/scheduled-strike-teams/issues/2) | 3 | 0 | ~2–4 days | |
| [HWiNFOterm](https://github.com/techrote/scheduled-strike-teams/issues/3) | 2 | 0 | ~1–3 days | |
| [INTUIT3D](https://github.com/techrote/scheduled-strike-teams/issues/4) | 2 | 0 | ~1–3 days | |
| [Steelmoth](https://github.com/techrote/scheduled-strike-teams/issues/5) | 4 | 0 | ~3–6 days | |
| [Flexdiffusion](https://github.com/techrote/scheduled-strike-teams/issues/7) | 3 | 3 initially; 1 active | #8 continues; #9/#10 owner acceptance/integration | PR #9 [88aadfa7](https://github.com/techrote/flexdiffusion/pull/9) Node/Chrome PASS; PR #10 [f789dc7](https://github.com/techrote/flexdiffusion/pull/10) UI/Chrome PASS; both merge HOLD |

*Indicative planning estimates, 13 November 2026. **Ideal workers** is estimated productive staffing if the project is prioritised independently, not the current share of the simultaneous 10-slot campaign. Days cover the team's agreed scope, exclude human-only gates, and are not release forecasts. “Last assigned” is a recent allocation snapshot, not a live task count. Milestones record verified progress when available; empty cells indicate none yet recorded. Actual live staffing and decisions are on the [campaign board](status/BOARD.md).*

### Historical references — not active teams

- [DashMinimix](https://github.com/techrote/scheduled-strike-teams/issues/6) — **abandoned and superseded by HWiNFOterm**. No workers, ETA or active backlog commitment; do not revive its PRs/issues as independent campaign targets.
- [Omnipanel](https://github.com/techrote/scheduled-strike-teams/issues/8) — **dormant / near-abandoned**. Retain as historical philosophical and architectural-intent reference for possible future projects; not an implementation queue.

## Operating limits

- **At most 10 concurrent active hourly tasks**, including existing schedules and monitors. The initial observed allocation was one enabled ShadeDoomVK CI A/B monitor and nine unallocated slots; re-check before scheduling.
- Strike teams may consist of **1–6 specialists**; generally start with one or two and only expand when ownership is genuinely separable.
- Workers are rotated out as soon as their bounded scope is qualified, requires a human action, or stops making meaningful progress. Do not keep them running for all 14 days by default.
- Use **1–5 manually triggered GPT-6 Pro engagements per complex team as needed**, for kickoff, troubleshooting, independent review and integration.
- **No autonomous merges or release publication.** Create/reuse Draft PRs, preserve project-specific safeguards and submit source-exact acceptance evidence for owner review.
- No unapproved security-setting changes, infrastructure deployments, secrets handling or physical-hardware acceptance claims.
- The canonical project issue and PR in each target repository remain authoritative for feature requirements. This hub records coordination, not a second competing specification.

## Status meaning

**Candidate** = selected for potential work; **Active** = an actual enabled task with a recorded ID; **Ready for owner review** = all automated and accessible technical gates for the scoped deliverable are satisfied, exact SHA and evidence linked; **Owner action needed** = a specific administrative or physical step blocks continuation; **Hold** = unresolved engineering or evidence defect; **Closed out** = owner has dispositioned the deliverable.

A *scoped PR ready for owner review* must not be counted as a *whole project release ready* unless its product release gates are independently satisfied.

## Reporting

Scheduled workers should update their **own team issue**, not repeatedly rewrite the board. A coordinator or owner updates the board after daily reviews (typically morning, midday and evening). Avoid issue duplication and prose-only claims of success: attach exact head SHA, checks and links. Keep historical snapshots dated rather than silently overwriting findings.

**Initial baseline:** 13 November 2026. **Schedule activation:** separate, owner-gated action; creating this repository does not authorise launching the proposed lineup.
