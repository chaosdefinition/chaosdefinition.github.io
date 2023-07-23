---
collection: publications
title: "Restricting Control Flow During Speculative Execution with Venkman"
permalink: /publication/2019-03-26-arXiv-Venkman
link: "https://doi.org/10.48550/arXiv.1903.10651"
classes: wide
bibtex:
  type: article
  id: Venkman@arXiv19
  author:
    - Shen, Zhuojia
    - Zhou, Jie
    - Ojha, Divya
    - Criswell, John
  title: "Restricting Control Flow During Speculative Execution with {Venkman}"
  journal: "arXiv preprint arXiv:1903.10651"
  url: "https://doi.org/10.48550/arXiv.1903.10651"
  doi: "10.48550/arXiv.1903.10651"
  archivePrefix: "arXiv"
  eprint: "1903.10651"
date: "2019-03-26"
pdf: "/assets/files/Venkman@arXiv19.pdf"
---

Side-channel attacks such as Spectre that utilize speculative execution to
steal application secrets pose a significant threat to modern computing
systems. While program transformations can mitigate some Spectre attacks, more
advanced attacks can divert control flow speculatively to bypass these
protective instructions, rendering existing defenses useless.

In this paper, we present *Venkman*: a system that employs program
transformation to completely thwart Spectre attacks that poison entries in the
Branch Target Buffer (BTB) and the Return Stack Buffer (RSB). Venkman
transforms code so that all valid targets of a control-flow transfer have an
identical alignment in the virtual address space; it further transforms all
branches to ensure that all entries added to the BTB and RSB are properly
aligned. By transforming all code this way, Venkman ensures that, in any
program wanting Spectre defenses, all control-flow transfers, including
speculative ones, do not skip over protective instructions Venkman adds to the
code segment to mitigate Spectre attacks.  Unlike existing defenses, Venkman
does not reduce sharing of the BTB and RSB and does not flush these structures,
allowing safe sharing and reuse among programs while maintaining strong
protection against Spectre attacks. We built a prototype of Venkman on an IBM
POWER8 machine. Our evaluation on the SPEC benchmarks and selected applications
shows that Venkman increases execution time to 3.47&times; on average and
increases code size to 1.94&times; on average when it is used to ensure that
fences are executed to mitigate Spectre attacks. Our evaluation also shows that
Spectre-resistant Software Fault Isolation (SFI) built using Venkman incurs a
geometric mean of 2.42&times; space overhead and 1.68&times; performance
overhead.
