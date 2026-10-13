---
title: "Kessler, The Alpha 21264 Microprocessor (IEEE Micro 1999)"
---
# Kessler, The Alpha 21264 Microprocessor (IEEE Micro 1999)

Richard Kessler’s IEEE Micro article is the fullest published description of the 21264 core, which the 21364 reuses unchanged apart from larger miss and victim buffers. It is the main academic source for the front end, branch prediction, renaming, issue queues, execution clusters, and the load and store queues.

[Read the open copy](https://acg.cis.upenn.edu/milom/cis501-Fall09/papers/Alpha21264.pdf) · [Publication page](https://doi.org/10.1109/40.755465).

**Primary source. Academic article (peer reviewed). Open copy on a University of Pennsylvania course page; the IEEE Xplore copy needs the UVA network.** Page numbers below are the printed IEEE Micro page numbers, 24–36.

## Where to look

- **Pipeline stages.** Figure 2 on p. 25 shows the seven stages, numbered 0–6: fetch, slot, rename, issue, register read, execute, and memory. The figure also labels the 20-entry integer and 15-entry floating-point issue queues, the two 80-entry integer register files, and the 72-entry floating-point file.
- **Fetch and line/way prediction.** Figure 3 on p. 26 and the surrounding text explain the line and way predictor, its 2-bit hysteresis, and how it is trained on cache fills and on jump targets.
- **Branch prediction.** The “Branch prediction” subsection on p. 26 gives the seven-cycle mispredict cost and the table sizes. Figure 4 on p. 28 is the tournament predictor block diagram (local history 1,024 × 10, local prediction 1,024 × 3, global 4,096 × 2, choice 4,096 × 2). The sidebar on p. 27 works through local and global examples.
- **Renaming and issue.** Figure 5 on p. 28 shows the map and queue stages with 80 in-flight instructions. Pages 28–29 cover the 31 + 41 register split, the two issue queues, the two arbiters, oldest-first selection, and in-order retirement.
- **Execution units and latencies.** Figure 6 on p. 30 shows the four integer pipes (two clusters) and two floating-point pipes with the unit in each. Table 1 on p. 30 gives retire pipe stages. Table 2 on p. 31 lists instruction latencies. The text on p. 30 explains the duplicated register file and the one-cycle cross-cluster penalty.
- **Memory system.** Pages 31–32 and Figure 8 describe the 32-entry load queue, 32-entry store queue, store-to-load forwarding, and the eight-entry miss address file. Figure 10 on p. 34 shows the store/load wait table. Figure 11 on p. 35 shows load hit/miss prediction and the two-cycle “minirestart.”

## BibTeX

{% raw %}
```bibtex
@article{kessler1999alpha21264,
  author = {Kessler, Richard E.},
  title = {The {Alpha} 21264 Microprocessor},
  journal = {IEEE Micro},
  volume = {19},
  number = {2},
  pages = {24--36},
  year = {1999},
  month = {March--April},
  doi = {10.1109/40.755465}
}
```
{% endraw %}

[Download all citations](../references.bib).
