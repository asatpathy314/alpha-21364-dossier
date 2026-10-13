---
title: "Alpha 21264 Microprocessor Hardware Reference Manual"
---
# Alpha 21264 Microprocessor Hardware Reference Manual

The hardware reference manual is the authoritative description of the 21264 core, and so of the 21364 core. Chapter 2, “Internal Architecture,” is the place to confirm any number from the papers: predictor table sizes, queue depths, pipeline stages, issue and retire rules, and the replay traps.

[Read the July 1999 edition](https://www.cs.tufts.edu/comp/150PAT/arch/alpha/21264hrm.pdf) · [21264/EV68CB edition, June 2001](https://classes.engineering.wustl.edu/cse362/images/a/af/Hrm_ev68cb_rev11.pdf) · [EV68CB edition at the Internet Archive](https://archive.org/details/dec-21264ev68cb_ev68dc_hrm).

**Primary source. Vendor documentation. Open copies on Tufts and Washington University course pages.** Locations below refer to the July 1999 edition, order number EC-RJRZA-TE. The Compiler Writer’s Guide says the 21364 core is the EV68CB core; the June 2001 EV68CB manual (DS-0031B-TE) has the same section numbers with small page shifts.

## Where to look

- **Block diagram.** Figure 2-1 on p. 2-3 shows the Ibox, Ebox, Fbox, Mbox and Cbox with the queues, register files, load and store queues, miss address file, and probe queue.
- **Branch predictor.** Section 2.1.1.2 and Figures 2-2 to 2-5, pp. 2-3–2-5: local predictor indexed by VPC bits 11:2, 12-bit global path history, and the choice table.
- **Fetch and return stack.** Section 2.1.1.4, pp. 2-5–2-6, describes octaword fetch, the line and set prediction bits stored with each fetch block, and the subroutine return prediction stack.
- **Rename and issue queues.** Sections 2.1.1.5–2.1.1.7, pp. 2-6–2-8: the rename maps, the 20-entry integer queue with its two arbiters, and the 15-entry floating-point queue with three arbiters. Section 2.1.1.9 gives the retire rate (8 sustained, 11 maximum).
- **Execution units and caches.** Sections 2.1.2–2.1.5, pp. 2-8–2-12: the integer clusters, floating-point unit, Cbox buffers, and the 64 KB two-way instruction and data caches.
- **Load and store handling.** Section 2.1.6, pp. 2-12–2-13, describes the 32-entry load queue, 32-entry store queue and 8-entry MAF. Section 2.7.1, pp. 2-23–2-24, covers load hit speculation and the 4-bit counter. Section 2.11, pp. 2-30–2-31, covers replay traps and the store-wait table.
- **Pipeline and rule tables.** Section 2.2 and Figure 2-8, pp. 2-13–2-16, with Table 2-1 (abort delays). Section 2.3 has Table 2-2 (pipes), Table 2-3 (slotting) and Table 2-4 (latencies), pp. 2-17–2-21. Table 2-5 on p. 2-21 gives retire rules.

## BibTeX

{% raw %}
```bibtex
@manual{compaq1999hrm,
  title = {Alpha 21264 Microprocessor Hardware Reference Manual},
  organization = {Compaq Computer Corporation},
  year = {1999},
  month = {July},
  note = {Order number EC-RJRZA-TE},
  url = {https://www.cs.tufts.edu/comp/150PAT/arch/alpha/21264hrm.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
