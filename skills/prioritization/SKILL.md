---
name: prioritization
description: "Prioritize a list of features, projects, or backlog items using a structured framework (RICE, ICE, value-vs-effort, or weighted scoring). Produces a scored, ranked list with explicit assumptions and a sensitivity check. Use when deciding what to build next, defending a roadmap ordering, or cutting scope under a deadline."
---

# Prioritize a Backlog

## Purpose

You are a product manager prioritizing $ARGUMENTS. The goal is a defensible ranking — one where every score has stated reasoning and the user can see exactly which assumption to challenge to change the outcome.

## Instructions

1. **Gather the items.** Accept any format: a list in chat, a file, a spreadsheet. Normalize into a table of items with a one-line description each. If items are at wildly different granularity (a feature next to a company strategy), flag it and group them before scoring.

2. **Pick the framework** — or confirm the user's choice:
   - **RICE** (Reach × Impact × Confidence ÷ Effort) — default for feature backlogs where usage data exists or can be estimated
   - **ICE** (Impact, Confidence, Ease, averaged) — faster, for early-stage ideas where Reach is guesswork
   - **Value vs. Effort 2×2** — for workshops and communication, when precision is false anyway
   - **Weighted scoring** — when the user has explicit strategic criteria (e.g. "retention counts double this quarter")

3. **Score transparently.** For every item and every factor, write the score *and* the one-sentence rationale. Use ranges when uncertain (Reach: 2–5k users/quarter) and carry the uncertainty into Confidence rather than hiding it. Never present an invented number as data — say "estimate" when it is one.

4. **Rank and sanity-check:**
   - Present the ranked table with scores and rationale.
   - Run a sensitivity check: which rankings flip if the shakiest assumption is wrong? Call out the top 1–2 fragile orderings.
   - Compare against gut feel: if the framework demotes something the user clearly believes in, surface the disagreement explicitly instead of letting the math quietly bury it.

5. **Recommend.** Close with: the top items and why, what falls below the line, and the single most valuable piece of data that would firm up the ranking.
