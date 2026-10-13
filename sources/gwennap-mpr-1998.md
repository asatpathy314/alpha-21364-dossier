---
title: "Gwennap, Alpha 21364 to Ease Memory Bottleneck (Microprocessor Report 1998)"
---
# Gwennap, Alpha 21364 to Ease Memory Bottleneck (Microprocessor Report 1998)

Linley Gwennap’s report on the 1998 announcement is the most readable description of why the 21364 was designed the way it was. It explains the memory-latency problem, the decision to reuse the 21264 core, the on-chip L2, the Direct RDRAM controllers, the directory in local memory, and the mesh network, with cost and die-size estimates.

[Read the open copy](https://www.ardent-tool.com/CPU/docs/MPR/19981026/121402.pdf) · [Mirror at UPC](https://studies.ac.upc.es/ETSETB/SEGPAR/microprocessors/21364%20(mpr).pdf).

**Secondary source. Trade press. Open copy at ardent-tool.com.** Microprocessor Report, 26 October 1998, four pages. The numbers are the 1998 targets; compare with the shipped chip in the [ISCA 2003 paper](cvetanovic-isca2003.md).

## Where to look

- **Motivation.** Page 1: memory latency as the bottleneck, and the decision to attach Direct RDRAM to the processor rather than a north bridge.
- **Core reuse.** Page 2, “Based on Existing 21264 CPU”: the core is reused with only a contemplated branch predictor tweak, while the miss buffer grows from 8 to 16 entries and the victim buffers to 16 + 16. The 12-cycle L2 latency is attributed partly to the reluctance to change the core.
- **Latency estimates and the mesh.** Page 2 and Figure 1: 90 ns local, 15 ns per hop, about 120 ns to a neighbor’s memory, 200 ns at four hops.
- **L2 and memory controllers.** Pages 2–3: 1.5 MB six-way L2 at 16 GB/s; the sidebar on RDRAM channels (four channels, 6 GB/s, 128 open pages per channel); the directory “uses part of the local memory to store the standard MESI coherency information.” Figure 2 on p. 3 is the chip block diagram.
- **Network and I/O.** Pages 3–4: four interprocessor ports of two unidirectional 16-bit links each, transit forwarding without CPU involvement, and the fifth port for the I/O chip. Page 4 has the die size, pin count, power and cost estimates.

## BibTeX

{% raw %}
```bibtex
@article{gwennap1998mpr,
  author = {Gwennap, Linley},
  title = {{Alpha} 21364 to Ease Memory Bottleneck: {Compaq} Will Add {Direct} {RDRAM} to 21264 Core for Late 2000 Shipments},
  journal = {Microprocessor Report},
  publisher = {MicroDesign Resources},
  year = {1998},
  month = {October},
  day = {26},
  pages = {1--4},
  url = {https://www.ardent-tool.com/CPU/docs/MPR/19981026/121402.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
