---
title: "Kessler, The Alpha 21264 Microprocessor"
---
# Kessler, The Alpha 21264 Microprocessor

The 21364 reuses the 21264 core, and this article is the fullest description of it: the pipeline, line and way prediction, the tournament branch predictor, renaming, the issue queues, the clustered execution units, and the load and store queues.

[Read the paper](https://acg.cis.upenn.edu/milom/cis501-Fall09/papers/Alpha21264.pdf) · [Publication page](https://doi.org/10.1109/40.755465).

Published in IEEE Micro 19(2), 1999, pp. 24–36. Page numbers are the printed ones.

## Where to look

- **Pipeline and fetch.** Figure 2 on p. 25 shows the seven stages. Figure 3 on p. 26 covers line and way prediction.
- **Branch prediction.** Page 26 gives the seven-cycle mispredict cost. Figure 4 on p. 28 shows the predictor with its table sizes.
- **Renaming and issue.** Figure 5 on p. 28 and pp. 28–29 cover the map, the 80-instruction window, and the two issue queues.
- **Execution units.** Figure 6 on p. 30 shows the clusters and units. Table 2 on p. 31 gives latencies.
- **Memory system.** Pages 31–35 cover the load and store queues, store-to-load forwarding, the wait table (Figure 10), and load hit/miss prediction (Figure 11).

## BibTeX

{% raw %}
```bibtex
@article{kesslerAlpha21264,
  author = {Kessler, Richard E.},
  title = {The {Alpha} 21264 Microprocessor},
  journal = {IEEE Micro},
  volume = {19},
  number = {2},
  pages = {24--36},
  year = {1999},
  doi = {10.1109/40.755465}
}
```
{% endraw %}

[Download all citations](../references.bib).
