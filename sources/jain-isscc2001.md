---
title: "Jain et al., A 1.2 GHz Alpha microprocessor with 44.8 GB/s chip pin bandwidth (ISSCC 2001)"
---
# Jain et al., A 1.2 GHz Alpha microprocessor with 44.8 GB/s chip pin bandwidth (ISSCC 2001)

The ISSCC paper is the circuit-level description of the 21364: process, clocking, the L2 cache arrays, and the high-speed Rambus and interprocessor pins. It is the source for the physical chip characteristics. It is two pages long and is cited by the IEEE Micro network paper as reference 2.

[IEEE Xplore](https://ieeexplore.ieee.org/document/912621) · [DOI](https://doi.org/10.1109/ISSCC.2001.912621).

**Primary source. Academic conference paper (peer reviewed). UVA network only; no open copy was found.** ISSCC 2001 Digest of Technical Papers, pp. 240–241. The abstract gives 1.75 MB L2, 130 million transistors, 0.18 µm seven-layer copper, 1.5 V, 125 W; the IEEE Micro paper later gives 152 million transistors, so note which figure you quote.

## Where to look

- **Chip characteristics.** The opening paragraph and the die photo for process, die size, transistor count, clock and power.
- **L2 cache circuits.** The description of the 1.75 MB array and its bandwidth; the companion paper by [Grodstein et al.](grodstein-glsvlsi2002.md) has more on the cache design.
- **Pin bandwidth.** The breakdown of the 44.8 GB/s across the Rambus channels, the four interprocessor ports and the I/O port.

## BibTeX

{% raw %}
```bibtex
@inproceedings{jain2001isscc,
  author = {Jain, Ashok and Anderson, William and Benninghoff, Tom and Bertucci, Dave and Braganza, Marco and Burnette, Jim and Chang, Tom and Eble, John and Faber, Rich and Gowda, Om and Grodstein, Joel and Hess, Greg and Kowaleski, John and Kumar, Ajay and Miller, Brian and Mueller, Ron and Paul, Patrick and Pickholtz, Jim and Russell, Steve and Shen, Mei and Truex, Tim and Vardharajan, Ajay and Xanthopoulos, Thucydides and Zou, Tim},
  title = {A 1.2 {GHz} {Alpha} microprocessor with 44.8 {GB/s} chip pin bandwidth},
  booktitle = {2001 IEEE International Solid-State Circuits Conference, Digest of Technical Papers},
  pages = {240--241},
  year = {2001},
  publisher = {IEEE},
  doi = {10.1109/ISSCC.2001.912621}
}
```
{% endraw %}

[Download all citations](../references.bib).
