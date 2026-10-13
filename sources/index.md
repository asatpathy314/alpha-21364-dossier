---
title: Sources
---
# Sources

Each page gives a short overview, useful places to look, the source’s type and access, and a BibTeX citation. You can also [download the full bibliography](../references.bib).

Three or more sources are primary and academic, as the assignment asks: Kessler (IEEE Micro 1999), Kessler, McLellan and Webb (ICCD 1998), Mukherjee et al. (IEEE Micro 2002), and Cvetanovic (ISCA 2003). The performance characterization sources are Cvetanovic’s two studies, the SPEC results, and the STREAM tables.

## Architecture and memory model

- [Alpha Architecture Handbook, Version 4 (Compaq, 1998)](alpha-architecture-handbook-v4.md)
- [McKenney, Is Parallel Programming Hard, And, If So, What Can You Do About It?](mckenney-perfbook.md)
- [Linux kernel, memory-barriers.txt](linux-memory-barriers.md)
- [LKML thread on Alpha read-side barriers, October 2001](lkml-2001-alpha-barriers.md)

## The 21264 core

- [Kessler, The Alpha 21264 Microprocessor (IEEE Micro 1999)](kessler-ieee-micro-1999.md)
- [Kessler, McLellan & Webb, The Alpha 21264 Microprocessor Architecture (ICCD 1998)](kessler-mclellan-webb-iccd1998.md)
- [Kessler, The Alpha 21264 Microprocessor (Hot Chips 10 slides, 1998)](kessler-hotchips10-1998.md)
- [Compiler Writer’s Guide for the 21264/21364 (Compaq, 2002)](compaq-compiler-writers-guide-21264-21364.md)
- [Alpha 21264 Microprocessor Hardware Reference Manual (Compaq, 1999)](compaq-21264-hardware-reference-manual.md)
- [Alpha 21264 Microprocessor Data Sheet (Compaq, 1999)](compaq-21264-data-sheet.md)

## The 21364 chip and systems

- [Mukherjee et al., The Alpha 21364 Network Architecture (IEEE Micro 2002)](mukherjee-21364-network-ieee-micro-2002.md)
- [Jain et al., A 1.2 GHz Alpha microprocessor with 44.8 GB/s chip pin bandwidth (ISSCC 2001)](jain-isscc2001.md)
- [Grodstein et al., the 1.75 MB L2 cache on the Alpha 21364 (GLSVLSI 2002)](grodstein-glsvlsi2002.md)
- [Bannon, Alpha 21364: A Scalable Single-chip SMP (Microprocessor Forum 1998)](bannon-21364-microprocessor-forum-1998.md)
- [Mukherjee, The Alpha 21364 and 21464 Microprocessors (Compaq slides)](mukherjee-21364-21464-slides.md)
- [HP AlphaServer ES47, ES80 and GS1280 Technical Summary (2003)](hp-gs1280-technical-summary-2003.md)

## Performance

- [Cvetanovic, Performance Analysis of the Alpha 21364-based HP GS1280 Multiprocessor (ISCA 2003)](cvetanovic-isca2003.md)
- [Cvetanovic, Performance Analysis of AlphaServer GS1280 (HP white paper, 2003)](cvetanovic-gs1280-white-paper-2003.md)
- [SPEC CPU2000 results for the AlphaServer GS1280](spec-cpu2000-gs1280.md)
- [STREAM benchmark results for the GS1280](stream-benchmark.md)

## Trade press

- [Gwennap, Alpha 21364 to Ease Memory Bottleneck (Microprocessor Report, 1998)](gwennap-mpr-1998.md)
- [Sites, It’s the Memory, Stupid! (Microprocessor Report, 1996)](sites-mpr-1996.md)
- [The Register, EV7 AlphaServers unleashed (2003)](register-ev7-launch-2003.md)

## Summary table

“Open” means the link opens without a login. “UVA only” means the publisher’s copy needs the UVA network or VPN. All links were checked on 12 October 2026.

| Source | Primary or secondary | Type | Access | What it covers |
|---|---|---|---|---|
| [Alpha Architecture Handbook, v4](alpha-architecture-handbook-v4.md) | Primary | Vendor ISA specification | Open | Registers, formats, extensions, MVI, LL/SC, MB/WMB, PALcode, memory ordering |
| [McKenney, perfbook](mckenney-perfbook.md) | Secondary | Book | Open | Memory ordering across CPU families; the Alpha section |
| [memory-barriers.txt](linux-memory-barriers.md) | Secondary | Kernel documentation | Open | Barrier types; the Alpha address-dependency case |
| [LKML thread, 2001](lkml-2001-alpha-barriers.md) | Secondary | Mailing list | Open | How the kernel learned about Alpha dependent-load reordering |
| [Kessler, IEEE Micro 1999](kessler-ieee-micro-1999.md) | Primary | Academic article | Open copy; UVA only at IEEE | Full 21264 core: pipeline, predictor, renaming, units, memory system |
| [Kessler et al., ICCD 1998](kessler-mclellan-webb-iccd1998.md) | Primary | Academic paper | Open copy; UVA only at IEEE | Short version of the above |
| [Kessler, Hot Chips 10](kessler-hotchips10-1998.md) | Secondary | Vendor conference slides | Open | Figures for the pipeline, predictor, queues, load prediction |
| [Compiler Writer’s Guide](compaq-compiler-writers-guide-21264-21364.md) | Primary | Vendor documentation | Open | What the 21364 changed; pipes, latencies, retire rules, replay traps |
| [21264 Hardware Reference Manual](compaq-21264-hardware-reference-manual.md) | Primary | Vendor documentation | Open | Authoritative core description, chapter 2 |
| [21264 Data Sheet](compaq-21264-data-sheet.md) | Secondary | Vendor datasheet | Open | Block diagram and pipeline summary |
| [Mukherjee et al., IEEE Micro 2002](mukherjee-21364-network-ieee-micro-2002.md) | Primary | Academic article | Open copy; UVA only at IEEE | Router, torus, virtual channels, deadlock avoidance, chip numbers |
| [Jain et al., ISSCC 2001](jain-isscc2001.md) | Primary | Academic paper | UVA only | Circuits, process, pin bandwidth, power |
| [Grodstein et al., GLSVLSI 2002](grodstein-glsvlsi2002.md) | Supplementary | Academic paper | UVA only | L2 cache design |
| [Bannon, Microprocessor Forum 1998](bannon-21364-microprocessor-forum-1998.md) | Secondary | Vendor presentation | Open (host unreachable at check time) | Goals, features, block diagrams, 1998 targets |
| [Mukherjee, 21364 and 21464 slides](mukherjee-21364-21464-slides.md) | Secondary | Vendor presentation | Open (host unreachable at check time) | Roadmap, 21364 summary, 21464 |
| [HP GS1280 Technical Summary](hp-gs1280-technical-summary-2003.md) | Secondary | Vendor documentation | Open | Systems, RIMMs, IO7, torus cabling, reliability |
| [Cvetanovic, ISCA 2003](cvetanovic-isca2003.md) | Primary | Academic paper (vendor author) | Open copy; UVA only at ACM | Performance characterization versus GS320 and ES45 |
| [Cvetanovic, HP white paper](cvetanovic-gs1280-white-paper-2003.md) | Secondary | Vendor white paper | Open | Longer study with other-vendor comparisons, I/O, tuning |
| [SPEC CPU2000, GS1280](spec-cpu2000-gs1280.md) | Primary | Published benchmark | Open | SPECint, SPECfp and rate results, 2003–2004 |
| [STREAM, GS1280](stream-benchmark.md) | Supplementary | Published benchmark | Open | Sustained memory bandwidth, 1 to 64 processors |
| [Gwennap, MPR 1998](gwennap-mpr-1998.md) | Secondary | Trade press | Open | Why the design, core reuse, L2, RDRAM, directory, mesh |
| [Sites, MPR 1996](sites-mpr-1996.md) | Secondary | Trade press | Open | Memory as the bottleneck; the motivation |
| [The Register, 2003](register-ev7-launch-2003.md) | Secondary | Trade press | Open | Launch, systems, prices, end of the line |

## Still to locate

- Krewell, “EV7 Stresses Memory Bandwidth,” Microprocessor Report, 24 March 2003. No open copy; Microprocessor Report after 2000 is behind the TechInsights paywall. Try the UVA library.
- Bannon, “Alpha 21364 (EV7),” Compaq slides, 4 January 2002. WikiChip hosts a PDF but the site could not be reached when this dossier was built.
- Bannon et al., GOMAC 2001, the paper the network article cites for the coherence protocol.
