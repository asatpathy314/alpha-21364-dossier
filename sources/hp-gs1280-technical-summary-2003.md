---
title: "HP AlphaServer ES47, ES80 and GS1280 Technical Summary"
---
# HP AlphaServer ES47, ES80 and GS1280 Technical Summary

HP’s technical summary describes the systems built around the 21364: the dual-processor module, the RDRAM channels and RIMMs, the IO7 I/O chip, the torus cabling, and the reliability features. It is the source for how I/O attaches and how the memory is organized at the board level.

[Read the open copy](https://www.cgl.ucsf.edu/Resources/gs1280/gs1280_ts.pdf).

**Secondary source. Vendor documentation. Open copy mirrored by UCSF.** Revision 1.0, 20 January 2003. Printed page numbers are used below; add two for the PDF page.

## Where to look

- **System overview.** Page 1: the EV7 as EV68 core plus two memory controllers, L2, one I/O port and four interprocessor ports; no central switch; 8-processor drawers and the 64-processor maximum.
- **Processor and memory.** Pages 2–3: 10.7 GB/s (1000 MHz) or 12.3 GB/s (1150 MHz) local memory bandwidth; 6.2 GB/s per interprocessor port; the router features; each Rambus controller drives four data channels plus a fifth parity channel; RIMM sizing.
- **IO7 chip.** Page 3 and page 7: the north port connects to the EV7 I/O port over two unidirectional paths; the four south ports are three PCI/PCI-X buses and one AGP; one IO7 per processor. The features table on p. 11 gives 3.2 GB/s of I/O bandwidth per processor.
- **Torus cabling.** Page 6: north–south and east–west cabling, 2P drawers as rings, 8P drawers using all four ports, and why square arrays perform best.
- **Reliability.** Pages 15–16: ECC on all processor-to-memory and processor-to-processor links, ECC on L1 and L2 data, RAID-style memory through the fifth channel, and coherence-engine checking that poisons data on illegal transitions.

## BibTeX

{% raw %}
```bibtex
@techreport{hp2003gs1280ts,
  author = {{Hewlett-Packard Company}},
  title = {{AlphaServer} {ES47}, {ES80}, and {GS1280} Systems: Technical Summary},
  institution = {Hewlett-Packard Company},
  year = {2003},
  month = {January},
  note = {Revision 1.0, 20 January 2003},
  url = {https://www.cgl.ucsf.edu/Resources/gs1280/gs1280_ts.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
