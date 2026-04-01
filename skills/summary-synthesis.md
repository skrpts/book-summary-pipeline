---
type: skill
id: summary-synthesis
title: Summary Synthesis
description: "Combines chapter-level summaries into a cohesive book summary with thematic analysis and critical evaluation"
tags: [Production, Academic, Learning, Writing]
connections:
  - target: llm-service
    type: runs_on
  - target: effective-summarisation-guide
    type: references
metadata:
  estimated_duration: "5-10 minutes"
  avg_tokens: 6000
---

## Capability

Takes the individual chapter summaries produced by earlier pipeline stages and synthesises them into a single, structured document. Goes beyond concatenation — identifies themes that span multiple chapters, traces how arguments develop through the book, and provides a critical evaluation of the work as a whole.

## Processing Approach

### Cross-Chapter Analysis

1. Map recurring themes, concepts, and terms across all chapter summaries
2. Identify how the author's central argument builds and evolves
3. Note any contradictions, shifts in position, or unresolved tensions
4. Track which chapters are foundational vs. which extend or apply the core ideas

### Synthesis Layers

The skill produces output at three levels of detail:

**Executive summary** (1 paragraph): The book's thesis, method, and contribution in a form you could explain to someone in two minutes.

**Standard summary** (1–2 pages): Chapter flow, key arguments, major evidence, and conclusions. Suitable for essay references or seminar preparation.

**Detailed summary** (3–5 pages): Everything above plus terminology glossary, notable quotes, methodology critique, and connections to the broader field.

The `summary_depth` input parameter controls which level is produced.

### Critical Evaluation

- Identifies the author's assumptions and methodological choices
- Notes what evidence is strong vs. where claims are under-supported
- Flags gaps — what the book doesn't address that a student should be aware of
- Suggests how the book relates to other major works in the field (when subject area is provided)

## When to Use

- After all chapters have been individually summarised
- When preparing for an essay, exam, or seminar discussion
- When you need to compare multiple books on the same topic

## Quality Criteria

- The executive summary must be self-contained — readable without the chapter breakdowns
- Thematic analysis must cite specific chapters, not make vague claims
- Critical evaluation must be balanced — acknowledge strengths alongside weaknesses
- Key takeaways must be actionable for revision, not just restatements of content
