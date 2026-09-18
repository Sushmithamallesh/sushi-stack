# Form chooser

Use this when you already have a question (or can write one). Output a recommendation: **form + metric + one-sentence why**, then the construction notes. Offer a runner-up if the question is still slightly wide.

## First fork: should this even be a chart?

| If the reader needs… | Use |
| --- | --- |
| Exact values, mixed units, lookup (“their” city), ranks, or comparison in two directions at once | **Table** (maybe with a bar in the key numeric column) |
| A pattern, trend, ranking, or distribution that prose would narrate poorly | **Chart** |
| A concept (period vs cohort, a definition, a mechanism) | **Annotated diagram** — geometry that carries the idea, labels that say it |
| Both “where on the map” and “what the distribution is” | **Two views** (e.g. choropleth + histogram) |
| “What share / how many / what risk” of the same thing | **A series of charts**, each titled as its own question — not one chart with three interpretations |

If a table would make the pattern obvious in under ten seconds, use the table. Charts earn their keep by making a comparison the eye can do.

## Question → form

Match the **verb** in the question.

| Question shape | Default form | Avoid |
| --- | --- | --- |
| How did X change over time? | Line if the quantity persists; columns if each period fills from zero or you have few aligned points | Dual-Y to magnify a same-unit series; arrows that imply the future will continue; a “trend” line on cross-sectional age/cohort data |
| How do a few categories compare on one measure? | Horizontal bars (labels stay readable). Cleveland dots are fine. | Vertical bars with rotated type; 3D bars; pies for close values |
| Who/what is biggest, in order? | Bars sorted by the value (or a meaningful order) | Alphabetical when the story is magnitude; visualizing rank as if 1 were half of 2 |
| How is 100% split? | Bars if shares must be compared; pie/donut only for one whole, ≤5 slices, near 25/50/75% | Pies for two polls; more than five slices; comparing slice areas |
| What are people dying of / composed of at each age/time? | Stacked or grouped bars, or lines of **shares** — only if share is the question | Treating share as risk |
| Do X and Y move together? | Scatter (then maybe a fit). If overlap hides the cloud, a 2D histogram | A reported *r* or *R*² as the figure |
| Two series, different units, “when this wiggled, did that?” | Dual-Y only if the audience can read it — or show the same measure in two units | Dual-Y for two dollar series; crossings treated as facts |
| What is the risk of X? | Rates, not counts, not shares | Counts that track population size |
| How many events happened? | Counts (and say the population context in the subtitle) | Rates passed off as volume |
| How is a quantity spread? | Histogram, dots, or ridgeline — then annotate the takeaway | Color alone on a map as a substitute for a distribution |
| Where is it high or low? | Map if geography is the mechanism; bars if geography is just labels | A map that makes similar values look wildly different because of a wild color scale |
| How does A differ from B, and the gap matters? | Range plot, or a chart of **A − B**, not only two steep lines | Two lines whose vertical gap is optically shrinking as they steepen |
| Many entities, each with its own trend | Small multiples, shared scale | One spaghetti chart with a 12-color legend |
| Many entities, compared to each other | One panel, direct labels, restrained color (grey + one highlight is often enough) | A unique color per state “so you can find them” |
| Unfamiliar but the right geometry (Lexis, heatmap, ridgeline) | That form **plus** a tiny how-to-read annotation on the figure | Dumping it on the reader with a caption on another page |

## Construction notes (once the form is picked)

**Labels.** Keep type horizontal. Label the data directly unless categories repeat everywhere (party colors on a constituency map) or there are too many to fit. Then: legend, in a logical or alphabetical order, with colors people already know when those associations exist.

**Panels.** Same scale across small multiples so “up” means the same thing. Split to let someone *follow* one series; combine to let them *compare*.

**Color.** Match the concept (vegetation, party, sea). Blue + orange, and lightness contrast. Second channel (label, dash, shape) so hue is not the only difference. Do not use red to mean “important” if it will be read as “bad.” No rainbow scales for continuous magnitudes.

**Uncertainty.** CIs for “how well we know the mean.” Prediction intervals, distributions, or example outcomes for “what happens to a person.” Absolute risks (or both absolute and relative) for lay risk.

**Standalone packing list.** Takeaway title. Subtitle in plain language: who, what, when, units. Footnote for sample size, definitions, caveats that change the reading. Source line. Link to data/code if it exists.

**Annotation.** If the chart type takes a tutorial, put the tutorial on the first panel or in the margin of the figure. Call out the one or two features they should not miss (a war, a law, a break in the series).

**When one view is insufficient.** Infant mortality by day vs cumulative deaths by day; map of prices vs histogram of prices. Do not cram both into one overloaded graphic if two quiet ones would be clearer.

## Mid-article script

Speak like an editor, not a dashboard vendor:

1. “The question this figure answers is: …”
2. “So the metric is …, not …, because …”
3. “Show it as … . A table/chart of … would hide …”
4. “On the figure itself, include … so it still makes sense alone.”
5. “People will misread … . Counter that by …”
