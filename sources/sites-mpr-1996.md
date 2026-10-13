---
title: "Sites, It’s the Memory, Stupid! (Microprocessor Report 1996)"
---
# Sites, It’s the Memory, Stupid! (Microprocessor Report 1996)

Richard Sites, one of the Alpha architects, wrote this short piece two years before the 21364 was announced. It argues from measurements that commercial workloads spend most cycles waiting on memory, which is the problem the 21364’s on-chip L2, memory controllers and router were built to attack. It is the standard citation for the design’s motivation.

[Read the open copy](http://www.cecs.uci.edu/~papers/mpr/MPR/ARTICLES/101004.pdf).

**Secondary source. Trade press. Open copy at UC Irvine (plain HTTP only).** Microprocessor Report, volume 10, number 10, 5 August 1996. The piece is a sidebar on pp. 2–3 of the seven-page feature “Architects Look to Processors of Future.”

## Where to look

- **The measurement.** TPC-C on a 200 MHz Pentium Pro and a 400 MHz Alpha 21164 ran at 4.2–4.5 cycles per retired instruction, so three of every four cycles retired nothing.
- **The argument.** Sites’s conclusion that memory latency and bandwidth, not the core, will set performance over the following decade. Compare with [Gwennap’s 1998 report](gwennap-mpr-1998.md), which opens with the same point.

## BibTeX

{% raw %}
```bibtex
@article{sites1996memory,
  author = {Sites, Richard L.},
  title = {It's the Memory, Stupid!},
  journal = {Microprocessor Report},
  volume = {10},
  number = {10},
  year = {1996},
  month = {August},
  day = {5},
  pages = {2--3},
  publisher = {MicroDesign Resources},
  url = {http://www.cecs.uci.edu/~papers/mpr/MPR/ARTICLES/101004.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
