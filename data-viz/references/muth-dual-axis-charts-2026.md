# What to consider when creating dual-axis charts

- **Author:** Lisa Charlotte Muth (Datawrapper)
- **URL:** https://www.datawrapper.de/blog/dual-axis-charts-guide
- **Date:** 2026-07-23
- **Good for:** The exception to “one scale.” When dual-Y is honest, and how it lies.

Dual-axis looks like a friendly line chart and is often **misread as one**. Scatterplots look hard; this looks easy and teaches the wrong lesson (“the revenue line is above units, so revenue is bigger”).

**Use only when units differ** (price vs volume, °C vs mm) *or* you are showing the **same measure in two units** (°C and °F — the safest case) *or* a Pareto (counts + cumulative share). Audience should already know the form, or the design has to scream that the axes are different.

**Do not** dual-axis two series in the **same unit** just because one is a short line. Readers remember “Lesotho above Uganda.” Shared-scale lines for the true picture; small multiples with free y if you must see wiggles.

Indexed (% change from a base) lets you compare slopes honestly. If you keep dual-Y, **align growth rates** of the two axes and **zero both** if either series is a bar/area. Avoid crossings — they are an artifact of scale choice, not a fact.

Make the trick visible: different geoms (line on columns), value labels with units, title that names both measures, colored axis ticks matching their series, legend that says “sales in $,” not “sales.” One series per side is already hard; five lines on stacked columns is abdication.

Prefer a split bar, a table, or small multiples when the chart is for a general reader.
