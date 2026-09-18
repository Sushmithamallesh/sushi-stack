# Saloni’s guide to data visualization

- **Author:** Saloni Dattani
- **URL:** https://www.scientificdiscovery.dev/p/salonis-guide-to-data-visualization
- **Date:** 2025-12-09 (correction 2025-12-11 on vertical writing in Mongolia, Taiwan, Japan)
- **Good for:** Why a chart exists; narrowing the question; clarity vs simplicity; guiding complex forms; standalone context; honest axes and metrics; reproducibility. Distilled for this skill — go to the URL for the original figures and full argument.

## Why bother

Charts earn space when they do a job prose does badly:

- **Explore** — patterns, breaks, and impossible points that averages hide (Anscombe; a coding error in a thesis supplement).
- **Explain a concept** — a small diagram can replace a long confused paragraph (period vs cohort on a Lexis diagram; a hook-shaped mortality curve split into disease vs external causes).
- **Carry a message** — memorable and shareable, which is also why misleading charts travel. Treat that as responsibility, not reach.

A bad chart is not a style problem. It is often the difference between understanding and anger. Redesigning a 3D meta-analysis bar chart into panels made the wide confidence intervals visible; the original’s depth had hidden the uncertainty. Prefer units people can sense-check (minutes, not only standardized mean differences) when the audience is broad.

## Guiding questions

Work through these, in order:

1. Is the chart type **meaningful** for a precise question?
2. Can I make it **clearer** (not necessarily simpler)?
3. If it is complicated, can I **guide** the viewer on the figure?
4. Does it work as a **standalone**, as far as possible?
5. Is the presentation **justifiable** (axis, color, metric, implication)?
6. Is it **reproducible** (source, ideally data and code)?

If choosing is painful, show multiple perspectives. “Choose both” is a valid answer.

## Meaningful type = precise question

Start from what you want to understand, then learn what the candidate metrics actually mean (TFR vs birth rate vs age-specific fertility is not a styling choice).

Broad question: “How do causes of death vary with age?” Three honest charts, three different questions:

- **Share** → what are people dying *from* at that age?
- **Count** → how *many* deaths from each cause?
- **Rate** → what is the *risk* of dying from each cause?

Present each as its own question. Do not let one stand in for the topic.

## Clearer, not dumber

Spend the reader’s effort on the data, not on decoding the graphic.

- Keep text **horizontal** (shorten names, wrap, or use horizontal bars). Keep bars vertical when height itself is the metaphor, or when a phone-shaped frame needs a vertical chart with horizontal type.
- **Label directly** unless there are many categories or one category maps onto many marks (an election map). Then a legend is fine; familiar party colors can make the legend optional.
- **Small multiples** when spaghetti hides every series. Same scale, easier to follow one country; harder to compare levels across countries — pick based on the question.
- **Second view** of the same data when one encoding fails (map of German property prices + histogram, because color is a poor magnitude scale).
- **Order** categories by inherent scale (agree → disagree) or alphabetically if there is no order.
- **Match color to concept.** Mismatched color is a Stroop test. Red/green “bad/good” will leak meaning you did not intend.
- **Color-blind friendly:** simulator (e.g. Coblis), a safe palette, direct labels. See Lisa Charlotte Muth’s writing on text and on color blindness.
- **Plain language** in the surrounding words so experts and non-experts can both think. Keep jargon when it distinguishes (mean vs median; iron-deficiency anemia vs anemia of chronic disease); then define it on the figure (`average (median)`; “external causes” plus examples).

## Guide the unfamiliar form

Heatmaps on Lexis plots, ridgelines, density plots can be the *right* geometry and still unread. Annotate:

- A mini how-to-read on the first panel (what x, y, and color mean).
- Takeaway notes beside a ridgeline so they do not have to remember the encoding while hunting for the story.

Trade-off: complexity vs time-to-read. Do not drop a clever form on the page with the tutorial in a different section.

## Standalone

Figures get screenshotted. Academic captions often bury the definition; news charts often omit how the thing was measured (survey vs diagnosis). Put the load-bearing context on the chart: takeaway title, plain-language metric, units, time, place, source, sample size when it matters. Pew-style packing (title = claim, subtitle = metric, footnote = method) is a model. If a caveat changes the reading, promote it — even if the title gets less catchy.

## Justifiable presentation (misreads)

- **Arrows on a line** can read as “and it will keep going that way.”
- **Color of land and sea** should match the world; a blue UK looks like a lake.
- **Y-axis crop vs full scale:** a tight crop on cherry-blossom dates exaggerates; a scale of the whole calendar year hides a real shift. Leave space so the min/max on the plot are not read as min/max possible. Include zero (or the true floor) when the data already live there. There is no moral victory in “always start at zero.”
- **Group averages** are not everyone’s risk. Relative suicide risk by diagnosis can alarm, hide heterogeneity, and get **confidence intervals** misread as the range of people. CIs are precision of the mean; prediction intervals (or raw percentages) speak to variation. People still see interval bands as spread ([Franconeri et al. 2021](https://doi.org/10.1177/15291006211051956) is the review she points to). Label clearly; prefer the form that matches the intended reading. Risk ratios can still be the right tool for association strength — with careful words.
- **Optical gap illusion:** two lines with a constant vertical difference look like they converge as they steepen. If the gap is the story, plot the difference or use a range plot (e.g. years from antibiotic discovery to clinical use).

## Transparent

A chart without a source is a vibe. Minimum: source on the figure, footnotes for the curious. Better: data, measurement notes, and code (her pattern: a URL on the chart to a repo folder per figure). Openness is how errors get found and how others remix.

## Tools she actually uses (optional)

Not a requirement for this skill. Her path: R + ggplot2 → SVG → Illustrator or Figma for annotation; Datawrapper for standard interactive bars, lines, maps, bubbles (strong defaults, fewer rotated labels in the wild). PowerPoint/Preview only for tiny tweaks.

## See also (now distilled next to this file)

The pieces this guide cites live as their own files in this folder. Start from `README.md`. Tufte’s books and paywalled examples are listed there under Skipped.
