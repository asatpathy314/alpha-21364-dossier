---
title: "McKenney, Is Parallel Programming Hard, And, If So, What Can You Do About It?"
---
# McKenney, Is Parallel Programming Hard, And, If So, What Can You Do About It?

The memory-ordering chapter compares CPU families in one table and treats Alpha as the most relaxed case. Use it to compare the Alpha model with x86, Arm and POWER, and for the explanation of dependent-load reordering.

[Book page](https://mirrors.edge.kernel.org/pub/linux/kernel/people/paulmck/perfbook/perfbook.html) · [PDF](https://kernel.org/pub/linux/kernel/people/paulmck/perfbook/perfbook.2026.06.21a.pdf).

These locations refer to release v2026.06.21a. The book is updated often; chapter numbers are more stable than pages.

## Where to look

- **Memory ordering.** Chapter 15 begins on p. 337. Sections 15.3.3–15.3.4, pp. 354–356, cover dependencies.
- **Comparison table.** Table 15.5 on p. 390.
- **Alpha.** Section 15.6.1, pp. 391–393, with Figure 15.27.

## BibTeX

{% raw %}
```bibtex
@book{mckenneyPerfbook,
  editor = {McKenney, Paul E.},
  title = {Is Parallel Programming Hard, And, If So, What Can You Do About It?},
  publisher = {kernel.org},
  year = {2026},
  note = {Release v2026.06.21a},
  url = {https://mirrors.edge.kernel.org/pub/linux/kernel/people/paulmck/perfbook/perfbook.html}
}
```
{% endraw %}

[Download all citations](../references.bib).
