---
title: "Compiler Writer’s Guide for the 21264/21364"
---
# Compiler Writer’s Guide for the 21264/21364

This is the one vendor document written for both chips, and it contains the only official statement of what the 21364 changed in the core. It also has the tables a compiler writer needs: which pipe runs each instruction class, latencies, retire rules, and the replay traps to avoid.

[Read the open copy](http://openwatcom.org/ftp/devel/docs/comp_guide_v2.pdf).

**Primary source. Vendor documentation. Open copy on the Open Watcom FTP mirror.** Part number EC-0100A-TE, revision 2.0, January 2002. Locations use the printed chapter-page numbers.

## Where to look

- **What the 21364 changed.** Section 1.3, pp. 1-4–1-6, says the 21364 “shares the same core as the 21264/EV68CB” except for an enlarged miss address file and victim address file, then lists the 21364 additions: 1.75 MB 7-way L2 with 12-cycle load-to-use, 15-entry MAF, 15-entry L1 victim buffer and 16-entry system victim buffer, 32-entry probe queue, two memory controllers, four-port network. Section 1.2 gives the 21264 list for comparison.
- **Register files and clusters.** Section 2.2 and Figure 2-1, pp. 2-2–2-3: the two integer clusters, the 31 + 8 PALshadow + 41 speculative split of the 80 entries, and the port counts. Section 2.3 and Figure 2-2 cover the 72-entry floating-point file.
- **Pipeline and abort delays.** Section 2.4 and Figure 2-3, pp. 2-4–2-6, walk through stages 0–6. Table 2-1, pp. 2-6–2-7, lists abort delays: 7 cycles for a branch mispredict, 8 for a JSR mispredict, 14 for a memory order trap.
- **Which pipe runs what.** Table 2-2, pp. 2-7–2-8, maps instruction classes to pipes L0, L1, U0, U1, FA, FM and FST. Table 2-3 gives slotting rules and Table 2-4, pp. 2-10–2-11, gives latencies.
- **Retire and replay traps.** Table 2-5, pp. 2-11–2-12, gives minimum retire latencies. Section 2.8, pp. 2-13–2-14, describes the load-load and store-load order traps and the 1,024-entry store-wait table.
- **Front end advice.** Section 3.4.2 lists instructions always predicted fall-through, 3.4.5 (p. 3-5) covers computed jumps and the return stack, and 3.9.1 (pp. 3-10–3-12) explains why only 33 integer and 37 floating-point physical registers are usable for in-flight results.

## BibTeX

{% raw %}
```bibtex
@manual{compaq2002cwg,
  title = {Compiler Writer's Guide for the 21264/21364},
  organization = {Compaq Computer Corporation},
  address = {Shrewsbury, MA},
  year = {2002},
  month = {January},
  note = {Part number EC-0100A-TE, revision 2.0},
  url = {http://openwatcom.org/ftp/devel/docs/comp_guide_v2.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
