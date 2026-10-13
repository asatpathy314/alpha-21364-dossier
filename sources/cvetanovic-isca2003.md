---
title: "Cvetanovic, Performance Analysis of the Alpha 21364-based HP GS1280 Multiprocessor (ISCA 2003)"
---
# Cvetanovic, Performance Analysis of the Alpha 21364-based HP GS1280 Multiprocessor (ISCA 2003)

This is the performance characterization source. It measures a GS1280 against the previous-generation GS320 and ES45 on latency, bandwidth, SPEC CPU2000, and applications, and it explains the results in terms of the on-chip L2, the memory controllers and the torus. Its system overview is also the clearest short statement of the chip’s cache and memory parameters. The author worked for HP, so read the comparisons with that in mind.

[Read the open copy](https://users.cs.utah.edu/~rajeev/cs7820/papers/alpha21364.pdf) · [ACM Digital Library](https://doi.org/10.1145/859618.859643) · [IEEE Xplore](https://ieeexplore.ieee.org/document/1207002).

**Primary source. Academic paper (peer reviewed), written by the vendor. Open copy on a Utah course page; the ACM and IEEE copies need the UVA network.** The open PDF has no printed page numbers. PDF page *n* is proceedings page 217 + *n*; both are given below.

## Where to look

- **System overview.** Section 2, PDF p. 2 (219), with Figures 2 and 3: 1.15 GHz; L2 of 1.75 MB, 7-way, 12-cycle (10.4 ns) load-to-use, 18.4 GB/s; 16 victim buffers; two RDRAM controllers at 12.3 GB/s with an optional fifth redundant channel; four interprocessor links at 6.2 GB/s; the directory-based forwarding protocol; and the GS320 switch-based design it replaces.
- **Local latency and bandwidth.** Section 3.1–3.2, PDF pp. 3–4 (220–221): Figure 4 (dependent-load latency against working set), Figure 5 (about 80 ns open page, about 130 ns closed page), Figures 6–7 (STREAM scaling).
- **Single-processor SPEC CPU2000.** Section 3.3, PDF pp. 4–5 (221–222), Figures 8–11: where the 21364 wins (swim) and where it loses to the GS320’s 16 MB off-chip L2 (facerec, ammp).
- **Remote latency.** Section 3.4, PDF p. 5 (222), Figure 13: local 83 ns, one hop 139–154 ns, two hops 175–195 ns, four hops 259 ns.
- **Interconnect under load and applications.** Sections 4–6, PDF pp. 6–9 (223–226): the load test, the “shuffle” rewiring, Fluent, NAS, GUPS, and memory striping.
- **Conclusions.** Sections 7–8 and Figure 28, PDF p. 10 (227): the summary of where the design wins and loses against the GS320.

## BibTeX

{% raw %}
```bibtex
@inproceedings{cvetanovic2003gs1280,
  author = {Cvetanovic, Zarka},
  title = {Performance Analysis of the {Alpha} 21364-based {HP} {GS1280} Multiprocessor},
  booktitle = {Proceedings of the 30th Annual International Symposium on Computer Architecture (ISCA '03)},
  address = {San Diego, CA},
  pages = {218--228},
  year = {2003},
  month = {June},
  publisher = {ACM},
  doi = {10.1145/859618.859643}
}
```
{% endraw %}

[Download all citations](../references.bib).
