---
title: Dossier
---
# A guide to the sources

The briefing splits the chip into four sections. This page says which sources answer each section’s questions and where to start. Every source page lists section and page numbers; the [sources index](sources/index.md) has the summary table with type, access, and what each one covers.

Several sources describe the 21364 as a 21264 core with a new memory system around it. That holds up: the [Compiler Writer’s Guide](sources/compaq-compiler-writers-guide-21264-21364.md), section 1.3, says the 21364 “shares the same core as the 21264/EV68CB” apart from a larger miss address file and victim buffers, and [Cvetanovic’s ISCA paper](sources/cvetanovic-isca2003.md) and the [network paper](sources/mukherjee-21364-network-ieee-micro-2002.md) say the same. [Gwennap’s 1998 report](sources/gwennap-mpr-1998.md) mentions a contemplated branch-predictor tweak that no later Compaq document confirms, so cite it as a plan, not a shipped change.

## Section A: overview, ISA, SIMD and memory consistency model

For the overview, start with [Gwennap’s report](sources/gwennap-mpr-1998.md) for the design’s motivation and the 1998 targets, then the first page of the [network paper](sources/mukherjee-21364-network-ieee-micro-2002.md) for the shipped numbers (152 million transistors, 0.18 µm, 1.2 GHz, 1.75 MB L2, up to 128 processors). [The Register](sources/register-ev7-launch-2003.md) gives the January 2003 launch, the systems, and the IBM fab. [Jain et al.](sources/jain-isscc2001.md) is the circuit paper for die size and power, behind the UVA library. The 1998 and shipped numbers differ (1.5 MB six-way versus 1.75 MB seven-way; 100 million versus 152 million transistors), so say which you are quoting.

For the ISA, the [Alpha Architecture Handbook](sources/alpha-architecture-handbook-v4.md) answers everything: registers and formats in chapter 3, PALcode in chapter 6, the extensions through the AMASK bits in Appendix D, the MVI multimedia instructions in section 4.13, and load-locked and store-conditional in section 4.2. The [Compiler Writer’s Guide](sources/compaq-compiler-writers-guide-21264-21364.md) says which units run the MVI instructions and their latency.

For the memory model, read handbook section 5.6 first, especially Table 5-1 and the dependence constraint in 5.6.1.7, which is why Alpha does not order dependent loads. Then [McKenney’s Table 15.5](sources/mckenney-perfbook.md) for the comparison with x86, Arm, POWER and the others, [memory-barriers.txt](sources/linux-memory-barriers.md) for the practical consequences, and the [2001 LKML thread](sources/lkml-2001-alpha-barriers.md) and Pugh’s note for the 21264 mechanism (invalidations waiting in the probe queue, flushed at every MB). The question of whether the implementation enforces more than the ISA requires is answered by that mechanism: the 21264 core really does exhibit the reordering.

## Section B: front end, register files and renaming

[Kessler’s IEEE Micro article](sources/kessler-ieee-micro-1999.md) is the main source: Figure 2 for the pipeline, Figure 3 for line and way prediction, Figure 4 for the tournament predictor, Figures 5 and 6 for renaming and the duplicated integer register file. The [ICCD paper](sources/kessler-mclellan-webb-iccd1998.md) is the short version, and the [Hot Chips slides](sources/kessler-hotchips10-1998.md) are the best figures to reuse. The [hardware reference manual](sources/compaq-21264-hardware-reference-manual.md), sections 2.1.1.2–2.1.1.5, confirms the table sizes and documents the return stack, which the papers do not mention. For the 21364 changes, cite the [Compiler Writer’s Guide](sources/compaq-compiler-writers-guide-21264-21364.md), section 1.3, and its section 3.9.1 for why only 33 of the 80 integer physical registers can hold in-flight results.

## Section C: back end and load/store handling

Start with [Kessler’s IEEE Micro article](sources/kessler-ieee-micro-1999.md), Figure 6 and Tables 1–2, for the units, clusters and latencies, and pp. 31–35 for the load and store queues, the wait table and load hit/miss prediction. The [Compiler Writer’s Guide](sources/compaq-compiler-writers-guide-21264-21364.md), Tables 2-2 to 2-5, maps every instruction class to its pipe and gives latencies and retire rules; section 2.8 covers replay traps. The [hardware reference manual](sources/compaq-21264-hardware-reference-manual.md), sections 2.1.1.6–2.1.1.7, 2.1.6, 2.7.1 and 2.11, is the authoritative version of the same material. Where latencies disagree (floating-point square root is 15/30 in the article and 18/33 in the manuals), prefer the manuals. The [data sheet](sources/compaq-21264-data-sheet.md) is background only.

## Section D: cache hierarchy, units outside the core, performance

For the caches and memory controllers, use [Cvetanovic’s ISCA paper](sources/cvetanovic-isca2003.md), section 2, for the shipped L2 (1.75 MB, seven-way, 12-cycle load-to-use), the two RDRAM controllers and the link bandwidths; the [Compiler Writer’s Guide](sources/compaq-compiler-writers-guide-21264-21364.md), section 1.3, for the victim and miss buffers; and the [hardware reference manual](sources/compaq-21264-hardware-reference-manual.md), section 2.1.5, for the 64 KB two-way L1 caches. [Grodstein et al.](sources/grodstein-glsvlsi2002.md) covers the L2 circuit design, behind the UVA library.

For the router, the [network paper](sources/mukherjee-21364-network-ieee-micro-2002.md) is the source: Figure 2 for the ports, pp. 28–31 for the torus, routing and the three deadlock cases, Figure 6 for the pipeline. For coherence, [Gwennap](sources/gwennap-mpr-1998.md) p. 3 says the directory lives in local memory, and the ISCA paper describes the forwarding protocol. For I/O and reliability, use the [HP technical summary](sources/hp-gs1280-technical-summary-2003.md), pp. 3, 7 and 15–16, and section 3.6 of the [white paper](sources/cvetanovic-gs1280-white-paper-2003.md).

For performance, the [ISCA paper](sources/cvetanovic-isca2003.md) and the [white paper](sources/cvetanovic-gs1280-white-paper-2003.md) are the characterization studies, written by HP. Pair them with the independent [SPEC CPU2000 results](sources/spec-cpu2000-gs1280.md) and the [STREAM tables](sources/stream-benchmark.md), both of which record the tested configuration. The design wins on bandwidth-bound codes and remote latency, and loses on working sets between 1.75 MB and 16 MB that fit the GS320’s off-chip L2.

## Using the references

Each [source page](sources/index.md) lists the relevant sections, figures, or tables and includes a copyable BibTeX entry. [Download the full bibliography](references.bib) to use all 23 entries in a LaTeX project.

Vendor manuals use chapter-page numbers; papers use the printed page numbers of the journal or proceedings. Two open PDFs lack printed numbers, and their pages give both the PDF page and the proceedings page.
