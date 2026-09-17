---
name: data-viz
description: Choose how to represent data in writing—chart vs table vs annotation, which metric, and which form. Use when drafting or editing articles with numbers, picking or reviewing a figure, captioning a chart, or when the user has data and is unsure how to show it.
---

# Data viz

You are choosing a **representation**, not decorating a chart. Pretty is a side effect of a precise question, the right metric, and a form the reader can read without a scavenger hunt.

This plate is for mid-article work: she has (or is about to have) numbers, and needs a call. Do not open with a generic “make a beautiful visualization.” Start with the question the figure must answer.

Sources live in `references/` (one file per article, plus an index). Load only what the decision needs. Add a new source by dropping a file and linking it from `references/README.md` — do not rewrite this skill to absorb it.

## How to work

1. **Name the question.** If it is a topic (“the baby boom”, “causes of death”), it is not a question yet. Narrow until one chart can be right or wrong.
2. **Pick the metric** that actually answers that question. Counts, rates, and shares of the same phenomenon answer different questions. Treat metric choice as part of the viz, not a later caption fix.
3. **Pick the form** with `playbooks/form-chooser.md`. Chart, table, annotated diagram, or more than one view. Say *why* that form, in one sentence she can keep or fight.
4. **Design for reading**, not for looking. Horizontal text, direct labels, familiar units, a title that states the takeaway, enough context that the figure survives a screenshot.
5. **Pre-empt the likely misread.** Axis zoom, color meaning, confidence intervals, group averages vs individuals. Fix the form or annotate; do not hope the body text will travel with the image.
6. **Leave a trail.** Source on the figure. Units on the figure. If code or data can be linked, link it.

If two honest questions remain, show two views. Choosing both is often better than forcing one clever chart.

## Defaults (break them on purpose)

- Prefer **familiar, practical units** (minutes, deaths per 100k, dollars) over unitless scores when a general reader has to judge size.
- Prefer **2D**. 3D bars and decorative depth hide uncertainty and make values unreadable.
- Prefer **one scale per comparison**. Dual axes for the same kind of quantity with mismatched scales is a trap.
- Prefer **direct labels** over a legend when each category appears once.
- Prefer **small multiples** when many series overlap; keep series on one panel when the point *is* the comparison.
- Prefer **plain language** in titles and axis labels, plus the precise term in parentheses when the jargon actually distinguishes something (`average (median)`).
- Prefer a **standalone figure**: title, what was measured, when, where, for whom, source. Charts get reshared without the paragraph underneath.

## What not to do

- Do not pick a chart type because it looks like “data viz” (pies for composition you cannot compare, 3D, rainbow legends for 40 lines).
- Do not stretch a y-axis to zero if that erases a real change; do not crop so tight that the floor looks like the minimum possible value. Leave air above and below the data; include zero when the data already sit near it.
- Do not treat confidence intervals as the spread of people. If the story is variation, show rates, distributions, or prediction intervals — not only precision of the mean.
- Do not run a Stroop test: red plants, blue land-as-sea, “bad” in the culture’s good color.
- Do not rotate labels to save a vertical bar chart; switch to horizontal bars, shorter names, or wrap.

## When you are stuck

Read `playbooks/form-chooser.md`. If the snag is honesty, units, or a known illusion, read `references/saloni-dattani-scientific-discovery-2025.md`. If a later source is on the index and fits better, read that instead of mashing everything into one answer.
