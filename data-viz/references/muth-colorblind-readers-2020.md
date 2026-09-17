# What to consider when visualizing data for colorblind readers

- **Author:** Lisa Charlotte Muth (Datawrapper)
- **URL:** https://www.datawrapper.de/blog/colorblindness-part2
- **Date:** 2020-06-23
- **Good for:** Encoding that still works when hue fails. Safer palettes, second channels, fewer colors.

About 4–5% of people have a color-vision deficiency. Most of this advice helps everyone.

- **Blue is the safest hue.** Pair blue with orange/red. Same-lightness green+red or green+blue collapses.
- **Get it right in black and white:** vary lightness, not only hue. Yellow is useful because it is so light. Brand red-on-dark can vanish for red-blind readers.
- Fewer colors beat a seven-color “safe” palette. More than three or four without labels makes people tune out. Grey + one or two highlights.
- Simulator (Coblis, Color Oracle, browser vision emulation) is a check, not proof. Encode a **second channel**: position, shape, dash, width, pattern, symbol (✔️), direct labels, hover highlight.
- Scatterplots: a few shapes, not confetti. Line charts: dash or weight where hues are close. Maps: pattern if two fills would collide.
- Direct labels remove the color-key problem.
- Hover that dims other series, or tooltips that name the category, is a web-only backup — not a print/screenshot backup.
- Ask an actual color-blind reader when the figure is load-bearing.

See also part 1 of the series (which combinations fail) if you need the perception background; this file is the construction list.
