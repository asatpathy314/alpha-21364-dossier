---
title: "Bannon, Alpha 21364: A Scalable Single-chip SMP (Microprocessor Forum 1998)"
---
# Bannon, Alpha 21364: A Scalable Single-chip SMP (Microprocessor Forum 1998)

Peter Bannon announced the 21364 at the 1998 Microprocessor Forum. The deck gives the goals, the feature list, the chip and system block diagrams, and the technology targets. Note that it describes the 1998 design point (1.5 MB six-way L2, 100 million transistors); the shipped chip had a 1.75 MB seven-way L2 and 152 million transistors.

[Slides at WikiChip](https://en.wikichip.org/w/images/5/56/ev7SMP.pdf) · [Transcription at SlideServe](https://www.slideserve.com/bathsheba/alpha-21364-a-scalable-single-chip-smp).

**Secondary source. Vendor presentation. The WikiChip PDF could not be reached when this dossier was built (connection refused), so the slide numbers below come from the SlideServe transcription. Re-check the PDF link before citing a slide number.** Bannon’s later deck, “EV7” at Microprocessor Forum in October 2001, is cited by Cvetanovic but no open copy was found.

## Where to look

- **Goals and roadmap.** Slides 3–4: the Alpha roadmap and the TPC-C motivation.
- **Feature list and block diagram.** Slides 5–6: the 21264 core with integrated L2, memory controllers and network interface. The block diagram is reproduced as Figure 2 in [Gwennap’s Microprocessor Report article](gwennap-mpr-1998.md).
- **L2 cache.** Slide 7: 1.5 MB, six-way, 16 GB/s, ECC, 12 ns load-to-use.
- **Memory controller.** Slide 8: Direct Rambus at 800 MHz, 6 GB/s, directory-based coherence, ECC.
- **Network interface.** Slide 9: 10 GB/s per processor, 15 ns processor-to-processor latency, out-of-order network with adaptive routing. Slide 10 is the system block diagram.
- **Technology.** Slide 11: 0.18 µm CMOS, 1000+ MHz, 100 W at 1.5 V, 100 million transistors.

## BibTeX

{% raw %}
```bibtex
@misc{bannon1998mpf,
  author = {Bannon, Peter},
  title = {{Alpha} 21364: A Scalable Single-chip {SMP}},
  howpublished = {11th Annual Microprocessor Forum, MicroDesign Resources, slides},
  year = {1998},
  month = {October},
  note = {Compaq Computer Corporation},
  url = {https://en.wikichip.org/w/images/5/56/ev7SMP.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
