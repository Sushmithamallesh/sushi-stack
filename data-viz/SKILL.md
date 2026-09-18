---
name: data-viz
description: Choose how to represent data in writing—chart vs table vs annotation, which metric, and which form. Use when drafting or editing articles with numbers, picking or reviewing a figure, captioning a chart, or when the user has data and is unsure how to show it.
---

# Data viz

You are choosing a **representation**, not decorating a chart. Pretty is a side effect of a precise question, the right metric, and a form the reader can read without a scavenger hunt.

This plate is for mid-article work: she has (or is about to have) numbers, and needs a call. Do not open with a generic “make a beautiful visualization.” Start with the question the figure must answer.

Sources live in `references/` (one file per article, plus an index). Load only what the decision needs. Add a new source by dropping a file and linking it from `references/README.md` — do not rewrite this skill to absorb it.

## How to work

1. **Name the question.** If it is a topic (“the baby boom”, “causes of death”), it is not a question yet. Narrow until one chart can be right or wrong. The **headline is a hypothesis** (`references/muth-questions-when-creating-charts-2017.md`).
2. **Pick the metric** that actually answers that question. Counts, rates, and shares of the same phenomenon are different figures (`references/dattani-four-charts-causes-of-death-2024.md`). Absolute vs relative vs odds are different sentences (`references/colnet-causal-measures-2023.md`). A correlation coefficient is not a picture of the data (`references/rohrer-whats-in-a-correlation-2025.md`).
3. **Pick the form** with `playbooks/form-chooser.md` and, if the shortlist is still wide, `references/muth-chart-types-guide-2025.md`. Chart, table, annotated diagram, or more than one view. Say *why* that form, in one sentence she can keep or fight.
4. **Prove the headline on the figure.** Add the comparison that makes the claim checkable. Grey + one highlight. Annotate the “why.” Direct labels, units on the marks, type people can read (`references/muth-text-in-visualizations-2022.md`).
5. **Pre-empt the likely misread.** Axis zoom, color meaning, CI-as-spread, group averages vs individuals, dual-Y crossings, rainbow scales. Fix the form or annotate; do not hope the body text will travel with the image.
6. **Leave a trail.** Source on the figure. Units on the figure. If code or data can be linked, link it.

If two honest questions remain, show two views. Choosing both is often better than forcing one clever chart.

## Defaults (break them on purpose)

- Prefer **familiar, practical units** over *d*, *r*, or other unitless scores when a general reader has to judge size (`references/vanhove-standardised-effect-sizes-2015.md`).
- Prefer encodings the eye can rank: **position on a shared scale**, then length, then area, then angle, then color intensity (`references/franconeri-visual-data-communication-2021.md`, `references/healy-look-at-data-socviz.md`).
- Prefer **2D**. 3D bars and decorative depth hide uncertainty and make values unreadable.
- Prefer **one scale per comparison**. Dual-Y only when units truly differ (or you are showing °C and °F), never to stretch a same-unit series (`references/muth-dual-axis-charts-2026.md`).
- Prefer **direct labels** over a legend when each category appears once.
- Prefer **small multiples** when many series overlap; keep series on one panel when the point *is* the comparison.
- Prefer **bars** (or a table) over pies when shares must be compared; pies only for one whole, few slices, quarters-ish (`references/datawrapper-dos-and-donts.md`).
- Prefer a **table** when the job is lookup, exact action, ranks, or two-way comparison (`references/muth-tables-2019.md`).
- Prefer **plain language** in the title, precision in the subtitle (`average (median)` when the jargon distinguishes).
- Prefer a **standalone figure**: takeaway title, what was measured, when, where, for whom, source.
- Prefer **blue/orange** and varying **lightness**; encode a second channel (label, dash, shape) so hue is not the only difference (`references/muth-colorblind-readers-2020.md`).

## What not to do

- Do not pick a chart type because it looks like “data viz” (pies for close shares, 3D, rainbow legends for 40 lines, stream graphs for exact values).
- Do not stretch a y-axis to zero if that erases a real change; do not crop so tight that the floor looks like the minimum possible value. Leave air above and below the data; include zero when the data already sit near it. Map bubble data to **area**, not diameter.
- Do not treat confidence intervals as the spread of people. If the story is a typical individual, draw prediction intervals, rates, or example outcomes (`references/hofman-goldstein-hullman-uncertainty-2020.md`).
- Do not lead a risk story with a relative change and no base rate.
- Do not run a Stroop test: red plants, blue land-as-sea, “bad” in the culture’s good color.
- Do not rotate labels to save a vertical bar chart; switch to horizontal bars, shorter names, or wrap.
- Do not title a figure with a correlation or a standardized effect as if that were the pattern.

## When you are stuck

| Snag | Read |
| --- | --- |
| Chart vs table vs which geometry | `playbooks/form-chooser.md`, then `references/muth-chart-types-guide-2025.md` |
| Counts vs rates vs shares | `references/dattani-four-charts-causes-of-death-2024.md` |
| Dual axis, pie, line, map | `references/muth-dual-axis-charts-2026.md` or `references/datawrapper-dos-and-donts.md` |
| Labels, title, units | `references/muth-text-in-visualizations-2022.md` |
| Color / colorblind | `references/muth-colorblind-readers-2020.md` |
| CIs, risk, illusions | `references/hofman-goldstein-hullman-uncertainty-2020.md`, `references/franconeri-visual-data-communication-2021.md` |
| *r*, *d*, absolute vs relative | `references/rohrer-whats-in-a-correlation-2025.md`, `references/vanhove-standardised-effect-sizes-2015.md`, `references/colnet-causal-measures-2023.md` |

Saloni’s umbrella notes remain in `references/saloni-dattani-scientific-discovery-2025.md`. Skipped links (paywall, books, examples) are listed in `references/README.md`.
