---
title: "Linux kernel, memory-barriers.txt"
---
# Linux kernel, memory-barriers.txt

The kernel’s memory-barrier document is written for programmers, and Alpha shaped it. It explains the barrier types, documents the address-dependency barrier that existed only because of Alpha, and ends with a section on what the Alpha gets up to. It is the best source for the practical consequences of the architecture’s memory model.

[Read the document](https://www.kernel.org/doc/Documentation/memory-barriers.txt).

**Secondary source. Kernel documentation. Open.** The file has no page numbers; locations are section headings in the current version. Authors in the header: David Howells, Paul E. McKenney, Will Deacon and Peter Zijlstra.

## Where to look

- **Guarantees.** The “Guarantees” section notes that on Alpha READ_ONCE also emits a memory-barrier instruction.
- **Address-dependency barriers.** “Address-dependency barriers (historical)” describes the now-removed smp_read_barrier_depends and states that, as of Linux 4.15, an smp_mb was added to READ_ONCE for Alpha. The worked example shows the anomaly the Alpha can exhibit.
- **Minimum ordering model.** “Assumed minimum execution ordering model” says the most relaxed case, the Alpha, must be assumed.
- **The Alpha section.** “The things CPUs get up to” and its subsection “And then there’s the Alpha” describe the split data cache and say the Alpha defines the kernel’s memory model.
- **References.** The closing list cites the Alpha AXP Architecture Reference Manual, chapters 5.2–5.6.

## BibTeX

{% raw %}
```bibtex
@misc{linux_memory_barriers,
  author = {Howells, David and McKenney, Paul E. and Deacon, Will and Zijlstra, Peter},
  title = {Linux kernel memory barriers},
  howpublished = {Linux kernel source, Documentation/memory-barriers.txt},
  url = {https://www.kernel.org/doc/Documentation/memory-barriers.txt},
  note = {Current version; record the kernel release when citing}
}
```
{% endraw %}

[Download all citations](../references.bib).
