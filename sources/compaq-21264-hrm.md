---
title: "Alpha 21264 Hardware Reference Manual"
---
# Alpha 21264 Hardware Reference Manual

The hardware reference manual is the authoritative description of the core. Chapter 2 is the place to confirm any number from the papers, and it documents the return stack and the caches, which the papers pass over.

[Read the manual](https://www.cs.tufts.edu/comp/150PAT/arch/alpha/21264hrm.pdf).

These locations refer to the July 1999 edition (EC-RJRZA-TE), using the printed chapter-page numbers.

## Where to look

- **Block diagram.** Figure 2-1 on p. 2-3.
- **Branch predictor and fetch.** Sections 2.1.1.2–2.1.1.4, pp. 2-3–2-6, including the return prediction stack.
- **Rename and issue queues.** Sections 2.1.1.5–2.1.1.9, pp. 2-6–2-8.
- **Caches and load/store queues.** Sections 2.1.5–2.1.6, pp. 2-11–2-13.
- **Load speculation and replay traps.** Section 2.7.1, pp. 2-23–2-24, and section 2.11, pp. 2-30–2-31.

## BibTeX

{% raw %}
```bibtex
@manual{compaq21264HRM,
  title = {{Alpha 21264 Microprocessor Hardware Reference Manual}},
  organization = {Compaq Computer Corporation},
  year = {1999},
  note = {EC-RJRZA-TE},
  url = {https://www.cs.tufts.edu/comp/150PAT/arch/alpha/21264hrm.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
