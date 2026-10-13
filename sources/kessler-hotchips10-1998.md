---
title: "Kessler, The Alpha 21264 Microprocessor (Hot Chips 10 slides)"
---
# Kessler, The Alpha 21264 Microprocessor (Hot Chips 10 slides)

Kessler’s Hot Chips talk is the best source of figures for the presentation. The slides repeat the pipeline block diagram, the line/set predictor, the tournament predictor, the map and queue structures, and the load hit-prediction timelines, all drawn more simply than in the papers.

[Read the slides](https://old.hotchips.org/wp-content/uploads/hc_archives/hc10/2_Mon/HC10.S1/HC10.1.1.pdf) · [Two-per-page copy at Duke](https://courses.cs.duke.edu/cps220/fall99/lectures/Alpha-21264.pdf) · [Hot Chips 10 program](https://hc10.hotchips.org/index.html).

**Secondary source. Conference slides from the vendor. Open copy in the Hot Chips archive.** The deck has 30 slides, each footed “REK August 1998”; slide numbers below are the footer numbers.

## Where to look

- **Highlights.** Slide 2 (600 MHz, 0.35 µm, 15 M transistors, 4-way integer and 2-way floating-point issue).
- **Block diagram.** Slides 3, 4, 9, 12 and 15 repeat the stage diagram with the 80 in-flight instructions, 32 loads, 32 stores, queue sizes, and the 80/80/72 register files.
- **Front end.** Slide 5 (speculating through 20 branches), slide 6 (line and set predictor), slides 7–8 (local versus global correlation, and the tournament predictor with table sizes).
- **Rename and issue.** Slides 10–11 (rename 4 per cycle, map CAMs, 20- and 15-entry queues, oldest-first collapsing queues).
- **Execution clusters.** Slides 13–14 list the units in each cluster and explain static upper/lower slotting with dynamic left/right cluster choice.
- **Memory.** Slides 16–17 (data cache and hazard detection), slides 18–19 (load hit and miss prediction timelines with the 4-bit counter), slides 20–21 (store/load hazard marking), slide 23 (off-chip latencies).

## BibTeX

{% raw %}
```bibtex
@misc{kessler1998hotchips,
  author = {Kessler, Richard E.},
  title = {The {Alpha} 21264 Microprocessor: Out-of-Order Execution at 600 {MHz}},
  howpublished = {Hot Chips 10 (HC10.1.1), Stanford University, slides},
  year = {1998},
  month = {August},
  note = {Compaq Computer Corporation},
  url = {https://old.hotchips.org/wp-content/uploads/hc_archives/hc10/2_Mon/HC10.S1/HC10.1.1.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
