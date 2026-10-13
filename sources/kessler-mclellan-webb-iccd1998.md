---
title: "Kessler, McLellan & Webb, The Alpha 21264 Microprocessor Architecture (ICCD 1998)"
---
# Kessler, McLellan & Webb, The Alpha 21264 Microprocessor Architecture (ICCD 1998)

This six-page conference paper is the shorter, earlier version of Kessler’s IEEE Micro article. It covers the same ground in less space and is the easiest open copy to hand to someone who wants the whole core on one read. A few numbers differ from the journal version, which is noted below.

[Read the open copy](https://portal.cs.umbc.edu/help/architecture/alpha21264a.pdf) · [Publication page](https://doi.org/10.1109/ICCD.1998.727028).

**Primary source. Academic paper (peer reviewed). Open author preprint hosted by UMBC; the IEEE Xplore copy needs the UVA network.** The preprint has no proceedings page numbers. Preprint page *n* is proceedings page 89 + *n*; both are given below.

## Where to look

- **Pipeline overview.** Section 1 (p. 1 / 90) names the stages, and Figure 1 (p. 2 / 91) is the block diagram with queue and register file sizes.
- **Line and set prediction.** Section 2.1 (p. 2 / 91). This paper says “set prediction” where the journal article says “way prediction.”
- **Branch prediction.** Section 2.2 (pp. 2–3 / 91–92) and Figure 2 (p. 3 / 92) give the tournament predictor and its table sizes. The text says the path history silo holds thirteen predictions (the journal says twelve) and that the core can speculate through up to 20 branches.
- **Renaming and issue queues.** Sections 3.1–3.2 (pp. 3–4 / 92–93): 41 speculative registers per file, 80-instruction window, 20- and 15-entry queues, static upper/lower slotting, two arbiters.
- **Execution engine.** Section 4 (p. 4 / 93) explains why the integer register file is duplicated (“as many as fourteen ports” otherwise) and Figure 3 shows the execution pipes.
- **Memory system.** Section 5 (p. 5 / 94) covers the double-pumped data cache, 32 loads and 32 stores in flight, section 5.1 the store/load wait table, and section 5.2 (pp. 5–6 / 94–95) load hit/miss prediction.

## BibTeX

{% raw %}
```bibtex
@inproceedings{kessler1998alpha21264,
  author = {Kessler, Richard E. and McLellan, Edward J. and Webb, David A.},
  title = {The {Alpha} 21264 Microprocessor Architecture},
  booktitle = {Proceedings of the 1998 IEEE International Conference on Computer Design: VLSI in Computers and Processors (ICCD '98)},
  address = {Austin, TX},
  pages = {90--95},
  year = {1998},
  month = {October},
  publisher = {IEEE Computer Society},
  doi = {10.1109/ICCD.1998.727028}
}
```
{% endraw %}

[Download all citations](../references.bib).
