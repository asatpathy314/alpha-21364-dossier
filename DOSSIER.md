---
title: Dossier
---
# A guide to the sources

The sources cover four broad topics: microarchitecture, the instruction set, the memory system, and performance. Here are some useful starting points for each.

## Microarchitecture

The 21364 reuses the 21264 core. Start with [Kessler’s article](sources/kessler-ieee-micro-1999.md) for the pipeline, branch predictor, register files, issue queues and load/store handling. The [hardware reference manual](sources/compaq-21264-hrm.md), chapter 2, confirms the numbers and adds the return stack and the caches.

Section 1.3 of the [Compiler Writer’s Guide](sources/compaq-compiler-writers-guide.md) states what the 21364 changed in the core. Its tables 2-2 to 2-5 map instruction classes to pipes and give latencies and retire rules.

## Instruction set

The [Alpha Architecture Handbook](sources/alpha-architecture-handbook-v4.md) is the specification. Chapter 3 covers registers and formats, Table D-3 the extension sets, section 4.13 the MVI multimedia instructions, section 4.2 load-locked and store-conditional, and chapter 6 PALcode.

## Memory system

For the on-chip L2, memory controllers and links, read section 2 of [Cvetanovic](sources/cvetanovic-isca2003.md). [Mukherjee et al.](sources/mukherjee-21364-network.md) covers the router, the torus and deadlock avoidance. [Gwennap](sources/gwennap-mpr-1998.md) explains the directory in local memory and the reasons for the design.

For memory ordering, start with section 5.6 of the [handbook](sources/alpha-architecture-handbook-v4.md), then Table 15.5 and section 15.6.1 of [McKenney](sources/mckenney-perfbook.md) for the comparison with other ISAs.

## Performance

[Cvetanovic](sources/cvetanovic-isca2003.md) measures the GS1280 against the GS320 and ES45. The study was written at HP; check the configuration before comparing with other systems.

## Using the references

Each [source page](sources/index.md) lists the relevant sections, figures, or tables and includes a copyable BibTeX entry. [Download the full bibliography](references.bib) to use all eight entries in a LaTeX project.

Manual references name a specific edition, and paper references use printed page numbers. Match those to the copy you are reading.
