---
title: "Cvetanovic, Performance Analysis of AlphaServer GS1280 (HP white paper)"
---
# Cvetanovic, Performance Analysis of AlphaServer GS1280 (HP white paper)

The white paper is the long form of the ISCA 2003 paper: 40 pages and 78 figures instead of 11 pages and 28. It adds comparisons with IBM, Sun, SGI and Itanium systems, an I/O performance section, a large application section, and configuration advice. It was written by HP for HP customers, so it is a vendor study.

[Read the open copy](https://hpc.ovgu.de/marvel/marvel_performance.pdf).

**Secondary source. Vendor white paper. Open copy mirrored by the University of Magdeburg HPC group.** January 2003, 40 pages; no HP document number is printed. Locations are PDF page numbers.

## Where to look

- **System diagrams.** Section 2, pp. 2–3: Figure 1a (EV7 interfaces: Rambus 2 × 6.2 GB/s, interprocessor 6.2 GB/s, I/O 3.1 GB/s to the IO7 chip), Figure 1b (dual-processor module with 20 RIMMs, 16 data and 4 redundancy), Figures 2a–2b (16- and 32-processor cabling).
- **Latency map.** Figure 13, p. 9: local 82 ns, one hop 133–150 ns, two hops 169–192 ns, three hops 215–228 ns, four hops 250 ns. These are slightly earlier numbers than the ISCA paper. Figure 12 on p. 8 shows read-dirty latency.
- **I/O.** Section 3.6, p. 11, Figures 17–19: how the IO7 attaches and what a drawer delivers.
- **Benchmarks against other vendors.** Figure 20 (SPEC CPU2000 peak, p. 12), Figures 21–22 (SPECrate, p. 13), Figure 23 (SPEComp, p. 14), Figure 24 (Linpack, p. 15, where the Alpha loses).
- **Configuration guidelines.** Section 6, pp. 32–37: ring versus torus, memory striping, one versus two populated memory controllers (Figure 75, p. 36), and I/O placement.
- **Conclusions and references.** Pages 38 and 40. The references include Bannon’s “EV7” Microprocessor Forum talk of October 2001 and an internal EV7 system design specification.

## BibTeX

{% raw %}
```bibtex
@techreport{cvetanovic2003whitepaper,
  author = {Cvetanovic, Zarka},
  title = {Performance Analysis of {AlphaServer} {GS1280}},
  institution = {Hewlett-Packard Company, AlphaServer Product Development},
  type = {White paper},
  year = {2003},
  month = {January},
  url = {https://hpc.ovgu.de/marvel/marvel_performance.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
