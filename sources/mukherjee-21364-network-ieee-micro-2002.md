---
title: "Mukherjee et al., The Alpha 21364 Network Architecture (IEEE Micro 2002)"
---
# Mukherjee et al., The Alpha 21364 Network Architecture (IEEE Micro 2002)

This is the main academic source on the 21364 itself rather than its core. It describes the on-chip router, the 2D torus, the packet classes, the virtual channels, and the deadlock-avoidance argument, and its opening page states the chip’s headline numbers. The authors are the Compaq designers.

[Read the open copy](https://pages.cs.wisc.edu/~markhill/restricted/ieeemicro02_21364network.pdf) · [Publication page](https://doi.org/10.1109/40.988687) · [Hot Interconnects 9 conference version](https://users.cs.utah.edu/~rajeev/cs7820/papers/alpha.pdf).

**Primary source. Academic article (peer reviewed). Open copy on Mark Hill’s Wisconsin page (the folder name says “restricted” but the file is served openly); the IEEE Xplore copy needs the UVA network.** Page numbers are the printed IEEE Micro pages, 26–35. The five-page Hot Interconnects version (DOI 10.1109/HIS.2001.946702) is shorter; prefer this one.

## Where to look

- **Headline numbers.** Page 26: 152 million transistors, 0.18 µm, 1.2 GHz; the 21264 core plus 1.75 MB L2, coherence hardware, two memory controllers and a router on one die; 12.8 GB/s local memory bandwidth; 22.4 GB/s router bandwidth; 13-cycle (10.8 ns) pin-to-pin router latency; up to 128 processors and 4 TB of memory. Figure 1 on p. 27 shows the floor plan and a 12-processor system.
- **Router ports.** Figure 2 on p. 27: eight input ports (north, south, east, west, cache, two memory controllers, I/O) and seven output ports.
- **Packet classes.** Pages 27–28: 39-bit flits (32 data + 7 ECC), 64-byte blocks in 16 flits, and the seven packet classes. Page 29 gives the class ordering used to keep coherence traffic deadlock free. Protocol details are deferred to a GOMAC 2001 paper by Bannon et al. (reference 4).
- **Topology and routing.** Page 28 and Figure 3 on p. 29: 2D torus with support for imperfect tori, virtual cut-through, buffering for 316 packets, minimal adaptive routing within the “minimum rectangle.”
- **Deadlock avoidance.** Pages 28–31, Figures 4 and 5: per-class virtual channels, Duato’s theory, the VC0/VC1 dimension-ordered escape channels, and the 19 virtual channels in total.
- **Router pipeline and arbitration.** Page 31 and Figure 6 for the pipeline and clock-forwarded 0.8 GHz links; Table 1 on p. 32 for input buffer allocation and the per-flit ECC policy; pp. 33–34 and Figure 7 for the local and global arbiters.

## BibTeX

{% raw %}
```bibtex
@article{mukherjee2002network,
  author = {Mukherjee, Shubhendu S. and Bannon, Peter and Lang, Steven and Spink, Aaron and Webb, David},
  title = {The {Alpha} 21364 Network Architecture},
  journal = {IEEE Micro},
  volume = {22},
  number = {1},
  pages = {26--35},
  year = {2002},
  month = {January--February},
  doi = {10.1109/40.988687}
}
```
{% endraw %}

[Download all citations](../references.bib).
