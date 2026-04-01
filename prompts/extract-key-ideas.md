---
type: prompt
id: extract-key-ideas
title: Extract Key Ideas
description: "Identifies the central arguments, evidence, and terminology from raw book text"
tags: [Production, Academic, Reading]
connections:
  - target: content-extraction
    type: derived_from
---

## Purpose

The first analytical prompt in the pipeline. Applied to the raw text (or a chunk of it) to pull out the building blocks that later stages will work with: what the author is arguing, what evidence they use, and what specialist terms they introduce.

## Prompt

You are an academic reading assistant. Analyse the following book text and extract its key components.

**Book:** {{input.book_title}} by {{input.book_author}}
**Subject area:** {{input.subject_area}}
**Section:** {{input.section_label}}

Extract the following from this text:

1. **Central argument(s):** What is the author claiming or asserting in this section? State each argument clearly in one sentence.

2. **Supporting evidence:** What evidence, examples, case studies, or data does the author use? Note whether each piece of evidence is empirical, anecdotal, theoretical, or cited from another source.

3. **Key terms and definitions:** List any specialist vocabulary the author introduces or relies on. Include their definitions as the author uses them (not dictionary definitions).

4. **Notable quotes:** Extract 2–3 direct quotes that best capture the author's voice or argument. Include enough context to understand them standalone.

5. **Assumptions:** What does the author take for granted or leave unstated? What prior knowledge does the reader need?

Format your response with clear headings for each section. Be precise — quote the text rather than paraphrase where accuracy matters.
