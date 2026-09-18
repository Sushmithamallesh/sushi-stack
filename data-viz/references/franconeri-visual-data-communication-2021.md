# The science of visual data communication: what works

- **Authors:** Steven L. Franconeri, Lace M. Padilla, Priti Shah, Jeffrey M. Zacks, Jessica Hullman
- **URL:** https://journals.sagepub.com/doi/10.1177/15291006211051956 (open PDF widely circulated; DOI `10.1177/15291006211051956`)
- **Date:** 2021
- **Good for:** Why some forms are slow or illusory. Ranked encodings, grouping, uncertainty, risk.

Review aimed at communicating to non-specialists, not expert-analysis UIs.

**See the data, not only the stats.** Same means/correlations can hide wildly different clouds (Anscombe; Datasaurus). Histograms and scatterplots before you trust a summary.

**Encoding rank (ratio judgments):** position on a common scale ≫ length ≫ area ≫ angle ≫ intensity. Stacked bars: only the baseline segment has position; the rest are length. Do not map two metrics to width×height of a rectangle (the eye sees area and aspect). Do not stack intensity on intensity. Circles: encode **area**, not diameter. Rainbow hue scales invent fake category boundaries at color-name edges.

**Fast vs slow:** the visual system grabs means and extrema in a glance. Comparing subsets is slow (a handful per second). Group so the intended comparison is the easy one; annotate/highlight the *one* comparison that carries the sentence. Presenters overestimate what others see.

**Memory:** legends tax working memory → direct labels. Unrelated chartjunk distracts; related pictorial bits can help memory. Animations usually confuse. New forms have a tuition — default to what the audience already knows. Respect “up = more,” “darker/more opaque = more.”

**Groups on a scatter:** color beats shape for finding a category; if you need two categorical encodings, color the important one.

**Uncertainty & risk:** error bars are read as the range of the data. For lay readers, show discrete outcomes (icon arrays, HOPs) rather than CI whiskers. Risk: **absolute** rates, frequencies (`3 in 10`) not relative (“30% more”), same denominator on icon arrays.

**Color vision:** pair red with **blue**, not green.

This is the paper behind Saloni’s steep-line gap illusion: if the difference is the story, plot the difference.
