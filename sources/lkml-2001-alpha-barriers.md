---
title: "LKML thread on Alpha read-side barriers, October 2001"
---
# LKML thread on Alpha read-side barriers, October 2001

This mailing-list thread is where the Linux kernel learned that the Alpha reorders dependent loads. Paul McKenney proposed lock-free list traversal, Richard Henderson pointed out that Alpha requires read-after-read barriers, and later messages quote Compaq’s own explanation. It is background, but it shows the model’s consequences in a real system.

[Original RFC, McKenney, 8 October 2001](https://lkml.iu.edu/hypermail/linux/kernel/0110.1/0239.html) · [Henderson’s reply](https://lkml.iu.edu/hypermail/linux/kernel/0110.1/0273.html) · [Russell’s message on partitioned caches](https://lkml.iu.edu/hypermail/linux/kernel/0110.1/0291.html) · [McKenney quoting Compaq](https://ratatoskr.run/lkml/2001/10/412226) · [Full thread](https://ratatoskr.run/lkml/2001/10/411742/t).

**Secondary source. Mailing-list archive. Open.** The thread is “RFC: patch to allow lock-free traversal of lists with insertion,” started 8 October 2001. A companion note by William Pugh, [Reordering on an Alpha processor](https://www.cs.umd.edu/~pugh/java/memoryModel/AlphaReordering.html), gives the litmus test and quotes Kourosh Gharachorloo of Compaq on the 21264 mechanism.

## Where to look

- **The problem.** McKenney’s RFC states that the Alpha WMB instruction is not sufficient for the reader side.
- **The architecture’s answer.** Henderson’s reply of 9 October: Alpha requires read-after-read barriers if ordering between reads is needed.
- **The mechanism.** Russell’s message quotes the explanation from Alpha architects that partitioned caches can process the invalidation of a pointer before the invalidation of what it points to.
- **Compaq’s documentation.** McKenney’s 10 October message quotes a Compaq patent and an OpenVMS note stating that Alpha provides coherent memory but no implicit ordering of reads and writes.
- **The outcome.** McKenney’s November 2001 patch introducing read_barrier_depends, which is an MB on Alpha and nothing elsewhere: [patch message](https://ratatoskr.run/lkml/2001/11/420058).
- **Pugh’s note.** The litmus test and Gharachorloo’s explanation that the 21264 flushes its incoming probe queue at every MB.

## BibTeX

{% raw %}
```bibtex
@misc{lkml2001alpha,
  author = {McKenney, Paul E. and Henderson, Richard and Russell, Rusty and others},
  title = {{RFC}: patch to allow lock-free traversal of lists with insertion},
  howpublished = {Linux kernel mailing list thread},
  year = {2001},
  month = {October},
  url = {https://lkml.iu.edu/hypermail/linux/kernel/0110.1/0239.html}
}
```
{% endraw %}

[Download all citations](../references.bib).
