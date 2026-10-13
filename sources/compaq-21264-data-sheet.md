---
title: "Alpha 21264 Microprocessor Data Sheet"
---
# Alpha 21264 Microprocessor Data Sheet

The data sheet is background only. Its short chapter 2 repeats the block diagram and the pipeline walk-through from the hardware reference manual, and the rest of the document covers signals, timing, and packaging. Use it when you want a compact statement of the microarchitecture without the rule tables.

[Read the open copy](https://datasheets.chipdb.org/DEC/21264/21264-Alpha.pdf).

**Secondary source. Vendor datasheet. Open copy at chipdb.org.** Order number EC-R4CFA-TE, revision 1.0, February 1999. Page numbers use the printed chapter-page format.

## Where to look

- **Microarchitecture summary.** Section 2.1 on p. 2-1 lists the boxes, and Figure 2-1 on p. 2-2 is the block diagram with queue, register file and buffer sizes.
- **Pipeline.** Section 2.2 and Figure 2-2, pp. 2-2–2-5, walk through stages 0–6 with the same wording as the hardware reference manual.
- **Implementation identity.** Section 2.4 on p. 2-7 gives the AMASK and IMPLVER values, which say which ISA extensions the chip implements.
- **Not here.** The issue, slotting, latency, retire and replay-trap tables are only in the hardware reference manual and the Compiler Writer’s Guide.

## BibTeX

{% raw %}
```bibtex
@manual{compaq1999datasheet,
  title = {Alpha 21264 Microprocessor Data Sheet},
  organization = {Compaq Computer Corporation},
  year = {1999},
  month = {February},
  note = {Order number EC-R4CFA-TE, revision 1.0},
  url = {https://datasheets.chipdb.org/DEC/21264/21264-Alpha.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
