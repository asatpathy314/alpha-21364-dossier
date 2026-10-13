---
title: "Alpha Architecture Handbook"
---
# Alpha Architecture Handbook

This is the ISA specification. Use it for the register set and instruction formats, the extension instructions, load-locked and store-conditional, PALcode, the barrier instructions, and the memory ordering rules in chapter 5.

[Read the handbook](http://www.o3one.org/hwdocs/alpha/alphaahb.pdf).

These locations refer to Version 4 (EC-QD2KC-TE, October 1998), using the printed chapter-page numbers.

## Where to look

- **Registers and formats.** Section 3.1, pp. 3-1–3-3, and section 3.3, pp. 3-10–3-14.
- **Extensions.** Table D-3, p. D-3, lists the AMASK bits for BWX, FIX, CIX and MVI. The MVI multimedia instructions are in section 4.13, pp. 4-151–4-156.
- **Atomics.** LDx_L in 4.2.4, p. 4-9, and STx_C in 4.2.5, p. 4-12, with examples in 5.5.2–5.5.3.
- **Barriers.** MB in 4.11.7, p. 4-142; WMB in 4.11.11, p. 4-147.
- **Memory ordering.** Section 5.6 begins on p. 5-10. Table 5-1 on p. 5-13 gives the issue constraints, 5.6.1.7 on p. 5-15 the dependence constraint, and pp. 5-17–5-21 the litmus tests.
- **PALcode.** Chapter 6, pp. 6-1–6-8.

## BibTeX

{% raw %}
```bibtex
@manual{alphaHandbook,
  title = {{Alpha Architecture Handbook}},
  organization = {Compaq Computer Corporation},
  edition = {Version 4},
  year = {1998},
  note = {EC-QD2KC-TE},
  url = {http://www.o3one.org/hwdocs/alpha/alphaahb.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
