# Risk ratio, odds ratio, risk difference… which causal measure is easier to generalize?

- **Authors:** Bénédicte Colnet, Julie Josse, Gaël Varoquaux, Erwan Scornet
- **URL:** https://arxiv.org/abs/2303.16008
- **Date:** 2023 (revised 2025)
- **Good for:** Absolute vs relative vs odds on a figure — different sentences, different impressions.

Saloni links this under “metrics can be misinterpreted.” It is a methods paper, not a chart tutorial. The viz-relevant core:

The same two probabilities can be a **risk difference** (0.8 fewer migraine days; +2 deaths per 100), a **risk ratio** / excess relative risk, an **odds ratio**, **NNT** (1 / difference; infinite when the difference is ~0, ugly intervals), or a survival ratio.

Relative numbers feel bigger (physicians treat more; headlines prefer them). Heterogeneity also **depends on the scale**: a factor can move the ratio and not the difference, or the reverse. Only the **risk difference** cleanly separates treatment from baseline at both subgroup and population level in general. It is also the measure that generalizes with the lightest covariate adjustment.

NNT is hard to draw well. Odds ratios are a modelling convenience, not a public sentence.

**For this skill:** if the reader is a person deciding for themselves, show **absolute** risks (or both: “from 2% to 3%, a 50% increase”). If the sentence is association strength inside comparable groups, a ratio can stay — with the base rates on the same figure.
