---
title: "Grodstein et al., Power and CAD considerations for the 1.75 Mbyte, 1.2 GHz L2 cache on the Alpha 21364 CPU (GLSVLSI 2002)"
---
# Grodstein et al., Power and CAD considerations for the 1.75 Mbyte, 1.2 GHz L2 cache on the Alpha 21364 CPU (GLSVLSI 2002)

This short paper describes the design of the on-chip L2 cache, the largest new block on the 21364. It covers the array organization, power, and the CAD flow used to verify it. Use it when you need the L2 described from the circuit side rather than the system side.

[ACM Digital Library](https://dl.acm.org/doi/10.1145/505306.505308) · [DOI](https://doi.org/10.1145/505306.505308).

**Supplementary source. Academic conference paper (peer reviewed). UVA network only; no open copy was found.** Proceedings of the 12th ACM Great Lakes Symposium on VLSI, New York, April 2002, pp. 1–6.

## Where to look

- **Cache organization.** The introduction and first figure for the 1.75 MB array, its banking, and the 7-way associativity.
- **Power.** The sections on array power and the tag-before-data access that keeps the data arrays idle on a miss.
- **Verification.** The CAD sections for how timing and noise were checked at 1.2 GHz.

## BibTeX

{% raw %}
```bibtex
@inproceedings{grodstein2002l2,
  author = {Grodstein, Joel and Rayess, Rami and Truex, Tim and Shattuck, Lee and Lowell, Steve and Bailey, Dan and Bertucci, Dave and Bischoff, Gary and Dever, Dan and Gowan, Mike and Lane, Rich and Lilly, Brian and Nagalla, Kalyan and Shah, Rahul and Shriver, Eric and Yin, Shih-Hsin and Morton, Shannon},
  title = {Power and {CAD} considerations for the 1.75 {Mbyte}, 1.2 {GHz} {L2} cache on the {Alpha} 21364 {CPU}},
  booktitle = {Proceedings of the 12th ACM Great Lakes Symposium on VLSI (GLSVLSI '02)},
  address = {New York, NY},
  pages = {1--6},
  year = {2002},
  month = {April},
  publisher = {ACM},
  doi = {10.1145/505306.505308}
}
```
{% endraw %}

[Download all citations](../references.bib).
