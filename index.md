---
title: Home
---
# Alpha 21364 source dossier

This is a source dossier for the Compaq Alpha 21364 (EV7) processor. It brings together the ISA handbook, the 21264 core documents, two research articles on the chip, and a performance study, with a short guide to what each source covers and where to look.

The four main topics are: microarchitecture (pipeline, branch prediction, register files, issue queues, load and store queues); unique features of the ISA (PALcode, the extension sets, atomics); the memory system (on-chip L2, memory controllers, router, and the memory consistency model); and performance characterisation (latency, bandwidth, SPEC CPU2000 against the previous generation).

## Read

- [Dossier](DOSSIER.md): a guide to reading by topic.
- [Sources](sources/index.md): an overview of each source, with section and page references.
- [BibTeX bibliography](references.bib): citations to copy into a LaTeX project.
- [Slides](https://docs.google.com/presentation/d/1WvGQo2q5WV6Dmll6yt7QE_HVwqK8GCssBEF8JIf1iRI/edit?usp=sharing): a presentation on the Alpha 21364.

## Sources

- [Alpha Architecture Handbook, Version 4](sources/alpha-architecture-handbook-v4.md)
- [Compiler Writer’s Guide for the 21264/21364](sources/compaq-compiler-writers-guide.md)
- [Alpha 21264 Hardware Reference Manual](sources/compaq-21264-hrm.md)
- [Kessler, The Alpha 21264 Microprocessor (IEEE Micro 1999)](sources/kessler-ieee-micro-1999.md)
- [Mukherjee et al., The Alpha 21364 Network Architecture (IEEE Micro 2002)](sources/mukherjee-21364-network.md)
- [Cvetanovic, Performance Analysis of the Alpha 21364-based HP GS1280 Multiprocessor (ISCA 2003)](sources/cvetanovic-isca2003.md)
- [Gwennap, Alpha 21364 to Ease Memory Bottleneck (Microprocessor Report 1998)](sources/gwennap-mpr-1998.md)
- [McKenney, Is Parallel Programming Hard, And, If So, What Can You Do About It?](sources/mckenney-perfbook.md)
