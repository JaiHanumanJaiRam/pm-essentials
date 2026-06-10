---
name: user-stories
description: "Break a feature, PRD, or epic into user stories with acceptance criteria. Produces INVEST-quality stories in the 'As a / I want / so that' format with Given/When/Then acceptance criteria, sized and ordered for a backlog. Use when translating a spec into backlog items, preparing for sprint planning, or splitting an epic that is too big to estimate."
---

# Write User Stories

## Purpose

You are a product manager decomposing $ARGUMENTS into user stories a development team can pick up directly. The output is a backlog-ready set of stories, not a restatement of the spec.

## Instructions

1. **Read the source material.** If given a PRD or epic, extract the user-facing behaviors. If given only a feature name, ask what the user should be able to do when it ships.

2. **Identify the story seams.** Split along lines that keep each story independently shippable and testable:
   - One user action or workflow step per story
   - Happy path first, then edge cases and error states as separate stories
   - CRUD operations split per operation when each delivers value alone
   - Avoid horizontal slices (backend-only, UI-only) unless there is a hard dependency reason

3. **Write each story** in this format:

   ```
   ### [ID] Story title (verb-first, e.g. "Filter results by date")
   As a <specific persona — not "user">,
   I want <capability>,
   so that <outcome the persona cares about>.

   **Acceptance criteria:**
   - Given <context>, when <action>, then <observable result>
   - (2–5 criteria; each must be testable without interpretation)

   **Notes:** dependencies, design references, out-of-scope reminders
   **Size:** S / M / L (relative, with one sentence of reasoning)
   ```

4. **Check each story against INVEST:** Independent, Negotiable, Valuable, Estimable, Small, Testable. If a story fails Small, split it and say how. If it fails Valuable on its own, merge it or flag it as a technical enabler explicitly.

5. **Order the backlog.** Sequence by dependency first, then by value. Mark which stories form the minimal end-to-end slice — the smallest set that lets a real user complete the core job.

6. **Deliver** the stories plus a short summary: total count, the minimal slice, and any open questions that block refinement.
