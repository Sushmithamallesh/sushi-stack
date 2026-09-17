# How visualizing inferential uncertainty can mislead readers about treatment effects

- **Authors:** Jake M. Hofman, Daniel G. Goldstein, Jessica Hullman
- **URL:** https://www.dangoldstein.com/papers/Hofman_Goldstein_Hullman_Visualizing_Uncertainty_Mislead_Scientific.pdf
- **Date:** 2020 (CHI)
- **Good for:** Confidence intervals vs prediction intervals vs HOPs — which uncertainty to draw.

**Inferential** uncertainty (standard error, 95% CI): how well we know the mean; shrinks with n. **Outcome** uncertainty (SD, 95% prediction interval): how much individuals vary; does not shrink with n.

Scientists often draw CIs. Readers then overpay for a small treatment, overestimate probability of superiority, and **underestimate how much people vary**. Extra caption text about both intervals does not fix a CI picture. Rescaling the CI axis helps a little. **Prediction intervals** and **HOPs** (animated random draws) track the individual-level questions better.

Error bars are overloaded (SE vs SD vs CI) and even researchers botch overlap heuristics. Bars + error bars add “within-the-bar” bias — they plotted points.

**For this skill:** if the sentence is about a typical person, do not draw a CI. Draw spread, rates, or example outcomes. If the sentence is “is the average different,” a CI can stay — and say so on the figure, because it will still be screenshotted as a range.
