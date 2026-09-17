# What’s in a correlation?

- **Author:** Julia Rohrer
- **URL:** https://www.the100.ci/2025/07/28/whats-in-a-correlation/
- **Date:** 2025-07-28
- **Good for:** When not to chart (or title) a Pearson *r* as if it were “the effect.”

*r* mashes slope, SD of X, and leftover SD of Y. A “small correlation” can mean a small effect, an X that barely varies, or a Y kicked around by everything else. Comparing *r* across groups can be a different slope, different variance, or both — you cannot see which from the two numbers.

If the variables have units people understand (income, birth order as first vs later), prefer the **unstandardized** slope, or a semi-standardized “+0.2 SD of Y for first-borns.” Correlations are less bad when both scales are arbitrary *and* you are asking a predictive question in one sample.

Do not build a chart whose punchline is “the correlation is higher in women.” Plot the scatter (or the slopes) and, if you must standardize, **standardize on the same SD for everyone**, not within group.

Same mash-up lives in *R*², Cohen’s *d* (noise in the control arm changes *d*), and heritability. Fisher-*z* does not save you.

**For this skill:** Anscombe is the picture; this is why the picture is required. A correlation coefficient is not a representation of the data.
