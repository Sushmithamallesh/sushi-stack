# Look at data (from *Data Visualization: A Practical Introduction*)

- **Author:** Kieran Healy
- **URL:** https://socviz.co/01-look-at-data.html (book site: https://socviz.co/)
- **Date:** 2nd ed. draft on the site (accessed 2026); 1st ed. Princeton, 2018
- **Good for:** Perception-ranked encodings; why pictures beat tables of summaries; Tufte as taste, not law.

Saloni lists the book as further reading. Distilled from ch. 1 (principles), not the ggplot cookbook chapters.

- Plot the cloud. Identical correlations hide different processes; a regression can be one outlier (South Africa; a New Year’s week of 911 calls).
- Three different failures: **taste** (3D, shadows, junk), **data** (you plotted the wrong metric — e.g. share who answered “10/10” vs the mean on a 1–10 democracy item), **perception** (the channel cannot carry the comparison).
- Cleveland–McGill: people judge **position on a common scale** most accurately, then length, then angle/slope, then area, then volume/color. Pies and 3D bars lose on purpose. A bar graph of birth-decade groups can beat a “trend line” when the data are cross-sectional, not longitudinal.
- Tufte: maximize ideas per ink, tell the truth, skip decoration. Useful for deleting junk; **not** a command to strip labels and gridlines — the most minimal boxplot is the hardest to read. Memorable infographics can stick without being precise. Minard is a one-off, not a template.
- A clean graphic does not save a cherry-picked series. It can even halo it.
- Who is looking matters: journal vs public vs your own scratch plot.

Later chapters (skim if you are drawing the figure in R): Cleveland **dot plots** often beat bars for one number per category; maps are not always the right encoding for country data.
