---
title: "McKenney, Is Parallel Programming Hard, And, If So, What Can You Do About It?"
---
# McKenney, Is Parallel Programming Hard, And, If So, What Can You Do About It?

McKenney’s book has the clearest comparison of memory models across CPU families, and Alpha is its standing example of the most relaxed one. Use it to compare Alpha with x86, Arm, POWER and the others, and for the explanation of why Alpha alone reorders dependent loads.

[Book page](https://mirrors.edge.kernel.org/pub/linux/kernel/people/paulmck/perfbook/perfbook.html) · [PDF, release 2026.06.21a](https://kernel.org/pub/linux/kernel/people/paulmck/perfbook/perfbook.2026.06.21a.pdf).

**Secondary source. Book, freely licensed. Open.** Page numbers refer to release v2026.06.21a. The book is updated often, so the chapter numbers are more stable than the pages.

## Where to look

- **Memory ordering chapter.** Chapter 15, “Advanced Synchronization: Memory Ordering,” starts on p. 337. Sections 15.3.3–15.3.4, pp. 354–356, cover address and data dependencies, with the note that READ_ONCE did not order dependent loads on Alpha before Linux 4.15.
- **The comparison table.** Table 15.5, “Summary of Memory Ordering,” on p. 390 in section 15.6, has columns for Alpha, Armv7, Armv8, Itanium, MIPS, POWER, SPARC TSO and x86. The row “Dependent loads reordered?” is yes only for Alpha.
- **The Alpha section.** Section 15.6.1, pp. 391–393, with Listing 15.51 and Figure 15.27, explains the partitioned-cache mechanism behind the reordering and the kernel’s response.
- **Discussion.** Section 15.6.10, p. 398, draws the comparison together.

## BibTeX

{% raw %}
```bibtex
@book{mckenney2026perfbook,
  editor = {McKenney, Paul E.},
  title = {Is Parallel Programming Hard, And, If So, What Can You Do About It?},
  publisher = {kernel.org},
  year = {2026},
  note = {Release v2026.06.21a, 21 June 2026},
  url = {https://mirrors.edge.kernel.org/pub/linux/kernel/people/paulmck/perfbook/perfbook.html}
}
```
{% endraw %}

[Download all citations](../references.bib).
