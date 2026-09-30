---
name: revenue-engine-maturity-diagnostic
title: Revenue engine maturity diagnostic
description: |
  Use this skill when a company wants to know why its go-to-market is not producing predictable revenue, before it buys automation, AI, or more headcount. Scores the revenue engine on six dimensions (ICP definition, scoring, outreach, data quality, feedback loops, automation) against a five-level maturity model (Foundation, Systemized, Orchestrated, Predictive, Compound), places the company at the level its weakest dimension supports, and returns the specific gaps to close for the next level. Reach for it when someone says "GTM maturity assessment", "are we ready for AI SDRs", "why is pipeline unpredictable", "revenue engine audit", "what should we automate first", or "we work hard and still miss the number".
category: RevOps
tags: [RevOps, Sales, Marketing, Leadership]
---

Applies when a go-to-market team is putting in effort and still getting unpredictable revenue, or is about to invest in automation or AI. Produces a maturity level per dimension, one overall level, and a ranked list of the gaps that block the next level.

Most go-to-market strategies fail from a lack of system, not a lack of effort. This diagnostic finds where the system breaks. Its core rule: **a revenue engine runs at the level of its weakest dimension**, so the job is to find that dimension and fix it before anything built on top of it.

## The model

Five levels, each a precondition for the next:

| Level | Name | In one line |
|---|---|---|
| 1 | Foundation | A written ICP, a CRM of record, one channel, defined pipeline stages |
| 2 | Systemized | Documented ICP, basic scoring, templates, data protocols, monthly review |
| 3 | Orchestrated | Two or more channels in automated sequences, intent in scoring, weekly optimization |
| 4 | Predictive | Trigger-based workflows, calibrated scoring, human approval on top-tier accounts |
| 5 | Compound | Self-calibrating scoring, lead-level messaging, forecast variance under 15% |

Six dimensions are scored at every level: **ICP definition, lead scoring, outreach, data quality, feedback loops, automation.** The full criteria for each level, and the pass/fail checklist, are in `references/level-criteria.md`.

## Run the diagnostic

1. **Collect evidence, not answers.** For each dimension, ask to see the artifact: the ICP document, the scoring model, a live sequence, a duplicate count from the CRM, the notes from the last optimization review. A capability that cannot be shown is scored as absent. The evidence request for every dimension is in `references/evidence-and-interview.md`.
2. **Score each dimension separately.** Place every dimension at the highest level whose criteria it fully meets. Partial credit does not exist; "we are rolling that out" counts as not met.
3. **Set the overall level to the lowest dimension score.** A company with Level 3 outreach and Level 1 data quality is a Level 1 company running Level 3 outreach on bad data, which is worse than running Level 1 outreach.
4. **Name the binding gap.** The binding gap is the unmet criterion in the lowest-scoring dimension that the most other dimensions depend on. Data quality and ICP definition are usually binding, because scoring, outreach and automation all consume them. Five worked cases, four of them where the problem the company named was not the binding gap, are in `references/worked-examples.md`.
5. **Build the advancement plan for one level up, not five.** List only the actions that move the company to the next level, in dependency order. The advancement actions per level, and how engagement scope scales with maturity, are in `references/advancement-playbook.md`.
6. **Re-score on a cadence.** Baseline at the start, set a target level and a date, and track checklist completion weekly. Advancement is claimed only when every criterion of the next level is met.

## What good looks like

- **What the best operator notices first:** the gap between the most advanced dimension and the least advanced one. A wide spread is the signature of a team that bought tactics before it built a system: sequencing software on an undefined ICP, AI personalization on duplicate-ridden data. The spread predicts wasted spend better than the average level does.
- **The common mistake:** scoring the company at its best dimension, or at the average, and then prescribing Level 4 or Level 5 capabilities. Automation amplifies whatever it runs on; on a Level 1 foundation it produces more bad outreach, faster. Mediocre diagnostics recommend tools. Good ones recommend the next unmet criterion.
- **Over-placement is the default.** Companies describe their intended process, not the one that runs. Assume self-assessment runs high until an artifact proves otherwise.
- **How you know the output is good:** every dimension score cites the evidence it rests on; the overall level equals the lowest dimension; the plan names no more than one level of advancement; and a reader can see why each action comes before the next.

## Rules

- MUST score from observed evidence; a claim without an artifact scores as not met.
- MUST set the overall level to the lowest dimension score, never an average.
- MUST limit the advancement plan to the next level.
- NEVER recommend automation, AI-generated messaging or predictive scoring to a company below Level 3 on data quality or ICP definition.
- NEVER change any CRM record, sequence or scoring model during the diagnostic; it is read-only, and every change it recommends goes to a human for approval.
