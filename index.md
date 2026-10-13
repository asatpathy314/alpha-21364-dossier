---
title: Home
---
# Alpha 21364 source dossier

This is a source dossier for the Compaq Alpha 21364 (EV7), the last Alpha processor to ship. It brings together the ISA handbook, the 21264 core papers, the 21364 network and performance papers, vendor documents, benchmark results and trade press, with a short guide to what each source covers and where to look.

The 21364 reuses the 21264 (EV6) core and surrounds it with a 1.75 MB on-chip L2, two Direct Rambus memory controllers, and a router for a 2D torus of up to 128 processors. So the core questions lean on 21264 papers and the memory, network and performance questions on 21364 material.

The four main topics are: the instruction set and memory consistency model (Alpha ISA, PALcode, the BWX, FIX, CIX and MVI extensions, load-locked and store-conditional, MB and WMB, and the weakest memory model of any mainstream ISA); the core microarchitecture (seven-stage pipeline, tournament branch predictor, duplicated integer register files, two issue queues, load and store queues); the memory system (cache hierarchy, memory controllers, directory coherence, the router and its deadlock avoidance); and performance characterization (latency, bandwidth, SPEC CPU2000 and STREAM against the previous-generation GS320).

## Read

- [Dossier](DOSSIER.md): a guide to reading by topic, following the briefing’s four sections.
- [Sources](sources/index.md): an overview of each source, with section and page references, access notes, and a summary table.
- [BibTeX bibliography](references.bib): citations to copy into a LaTeX project.
- Slides: the Google Slides presentation will be linked here once the deck is ready.

## Sources

### Architecture and memory model

- [Alpha Architecture Handbook, Version 4 (Compaq, 1998)](sources/alpha-architecture-handbook-v4.md)
- [McKenney, Is Parallel Programming Hard, And, If So, What Can You Do About It?](sources/mckenney-perfbook.md)
- [Linux kernel, memory-barriers.txt](sources/linux-memory-barriers.md)
- [LKML thread on Alpha read-side barriers, October 2001](sources/lkml-2001-alpha-barriers.md)

### The 21264 core

- [Kessler, The Alpha 21264 Microprocessor (IEEE Micro 1999)](sources/kessler-ieee-micro-1999.md)
- [Kessler, McLellan & Webb, The Alpha 21264 Microprocessor Architecture (ICCD 1998)](sources/kessler-mclellan-webb-iccd1998.md)
- [Kessler, The Alpha 21264 Microprocessor (Hot Chips 10 slides, 1998)](sources/kessler-hotchips10-1998.md)
- [Compiler Writer’s Guide for the 21264/21364 (Compaq, 2002)](sources/compaq-compiler-writers-guide-21264-21364.md)
- [Alpha 21264 Microprocessor Hardware Reference Manual (Compaq, 1999)](sources/compaq-21264-hardware-reference-manual.md)
- [Alpha 21264 Microprocessor Data Sheet (Compaq, 1999)](sources/compaq-21264-data-sheet.md)

### The 21364 chip and systems

- [Mukherjee et al., The Alpha 21364 Network Architecture (IEEE Micro 2002)](sources/mukherjee-21364-network-ieee-micro-2002.md)
- [Jain et al., A 1.2 GHz Alpha microprocessor with 44.8 GB/s chip pin bandwidth (ISSCC 2001)](sources/jain-isscc2001.md)
- [Grodstein et al., the 1.75 MB L2 cache on the Alpha 21364 (GLSVLSI 2002)](sources/grodstein-glsvlsi2002.md)
- [Bannon, Alpha 21364: A Scalable Single-chip SMP (Microprocessor Forum 1998)](sources/bannon-21364-microprocessor-forum-1998.md)
- [Mukherjee, The Alpha 21364 and 21464 Microprocessors (Compaq slides)](sources/mukherjee-21364-21464-slides.md)
- [HP AlphaServer ES47, ES80 and GS1280 Technical Summary (2003)](sources/hp-gs1280-technical-summary-2003.md)

### Performance

- [Cvetanovic, Performance Analysis of the Alpha 21364-based HP GS1280 Multiprocessor (ISCA 2003)](sources/cvetanovic-isca2003.md)
- [Cvetanovic, Performance Analysis of AlphaServer GS1280 (HP white paper, 2003)](sources/cvetanovic-gs1280-white-paper-2003.md)
- [SPEC CPU2000 results for the AlphaServer GS1280](sources/spec-cpu2000-gs1280.md)
- [STREAM benchmark results for the GS1280](sources/stream-benchmark.md)

### Trade press

- [Gwennap, Alpha 21364 to Ease Memory Bottleneck (Microprocessor Report, 1998)](sources/gwennap-mpr-1998.md)
- [Sites, It’s the Memory, Stupid! (Microprocessor Report, 1996)](sources/sites-mpr-1996.md)
- [The Register, EV7 AlphaServers unleashed (2003)](sources/register-ev7-launch-2003.md)
