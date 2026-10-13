---
title: "Alpha Architecture Handbook, Version 4"
---
# Alpha Architecture Handbook, Version 4

The handbook is the ISA specification. It is the source for the register set, instruction formats, the extension instructions the 21364 implements (BWX, FIX, CIX and the MVI multimedia set), load-locked and store-conditional, PALcode, the MB and WMB barriers, and chapter 5’s memory ordering rules with their litmus tests. Nearly every Section A question is answered here.

[Read the open copy](http://www.o3one.org/hwdocs/alpha/alphaahb.pdf) · [Alpha Architecture Reference Manual, 4th ed. (2002)](http://download.majix.org/dec/alpha_arch_ref.pdf).

**Primary source. Vendor ISA specification. Open copy mirrored at o3one.org.** Order number EC-QD2KC-TE, October 1998, 371 pages. The 2002 Architecture Reference Manual on the second link has the same Part I section numbers with slightly different page numbers, and is the edition the Linux documentation and McKenney cite. Page numbers below use the handbook’s chapter-page format.

## Where to look

- **Registers and formats.** Section 3.1, pp. 3-1–3-3, covers the integer and floating-point registers, the lock registers, and the cycle counter. Section 3.3, pp. 3-10–3-14, gives the memory, branch, operate, floating-point and PALcode instruction formats.
- **Extensions.** Section 4.1, pp. 4-1–4-3, states the subsetting and emulation rules. Table D-3 on p. D-3 lists the AMASK bits: BWX (byte and word loads and stores), FIX (float-to-integer moves and square root), CIX (count instructions), and bit 8, MVI, the multimedia instructions. AMASK is described at 4.11.1, p. 4-133, and IMPLVER at 4.11.6, p. 4-141.
- **SIMD.** Section 4.13, “Multimedia (Graphics and Video) Support,” pp. 4-151–4-156: packed byte and word minimum and maximum, pixel error, pack and unpack, all on the 64-bit integer registers. Note that the handbook calls this set MVI, not MAX, and that it has no packed add, multiply, or floating-point forms.
- **Atomics.** LDx_L at 4.2.4, p. 4-9, and STx_C at 4.2.5, p. 4-12. Worked examples in 5.5.2–5.5.3, pp. 5-6–5-7, and the formal rules in 5.6.1.8, p. 5-16.
- **Barriers.** MB at 4.11.7, p. 4-142; WMB at 4.11.11, p. 4-147; EXCB at 4.11.4 and TRAPB at 4.11.9; CALL_PAL IMB at 6.7.3, p. 6-8.
- **Memory model.** Section 5.6, “Read/Write Ordering,” starts on p. 5-10. Table 5-1 on p. 5-13 gives the processor issue constraints; 5.6.1.7 on p. 5-15 defines the dependence constraint, which only runs from a read to a later write and so leaves dependent loads unordered. Litmus tests 1–11 are on pp. 5-17–5-21; implied barriers and software implications follow on pp. 5-22–5-29.
- **PALcode.** Chapter 6, pp. 6-1–6-8: what PALcode is, its environment, the required functions, and replacement. The CALL_PAL instruction is at 4.11.2, p. 4-135.

## BibTeX

{% raw %}
```bibtex
@manual{compaq1998handbook,
  title = {Alpha Architecture Handbook},
  organization = {Compaq Computer Corporation},
  edition = {Version 4},
  year = {1998},
  month = {October},
  note = {Order number EC-QD2KC-TE},
  url = {http://www.o3one.org/hwdocs/alpha/alphaahb.pdf}
}
```
{% endraw %}

[Download all citations](../references.bib).
