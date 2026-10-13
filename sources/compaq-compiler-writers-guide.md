---
title: "Compiler Writer’s Guide for the 21264/21364"
---
# Compiler Writer’s Guide for the 21264/21364

This is the one vendor document written for both chips. It states what the 21364 changed in the core, and it has the tables for which pipe runs each instruction class, latencies, retire rules, and replay traps.

[Read the guide](http://openwatcom.org/ftp/devel/docs/comp_guide_v2.pdf).

These locations refer to revision 2.0 (EC-0100A-TE, January 2002), using the printed chapter-page numbers.

## Where to look

- **21364 changes.** Section 1.3, pp. 1-4–1-6: the same core as the 21264/EV68CB apart from larger miss and victim buffers, plus the 1.75 MB 7-way L2, memory controllers and network.
- **Register files.** Sections 2.2–2.3, pp. 2-2–2-4, with Figures 2-1 and 2-2.
- **Pipeline.** Section 2.4, pp. 2-4–2-6. Table 2-1 gives abort delays.
- **Pipes and latencies.** Table 2-2, pp. 2-7–2-8, maps instruction classes to pipes. Table 2-4, pp. 2-10–2-11, gives latencies. Table 2-5 gives retire latencies.
- **Replay traps.** Section 2.8, pp. 2-13–2-14, and section 3.7.

## BibTeX

{% raw %}
```bibtex
@manual{compaqCompilerGuide,
  title = {{Compiler Writer's Guide for the 21264/21364}},
  organization = {Compaq Computer Corporation},
  year = {2002},
  note = {EC-0100A-TE, revision 2.0},
  url = {http://openwatcom.org/ftp/devel/docs/comp_guide_v2.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
