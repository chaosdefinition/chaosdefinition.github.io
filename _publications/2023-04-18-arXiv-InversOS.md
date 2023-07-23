---
collection: publications
title: "InversOS: Efficient Control-Flow Protection for AArch64 Applications with Privilege Inversion"
permalink: /publication/2023-04-18-arXiv-InversOS
link: "https://doi.org/10.48550/arXiv.2304.08717"
classes: wide
bibtex:
  type: article
  id: InversOS@arXiv23
  author:
    - Shen, Zhuojia
    - Criswell, John
  title: "{InversOS}: Efficient Control-Flow Protection for {AArch64} Applications with {Privilege Inversion}"
  journal: "arXiv preprint arXiv:2304.08717"
  url: "https://doi.org/10.48550/arXiv.2304.08717"
  doi: "10.48550/arXiv.2304.08717"
  archivePrefix: "arXiv"
  eprint: "2304.08717"
date: "2023-04-18"
pdf: "/assets/files/InversOS@arXiv23.pdf"
---

With the increasing popularity of AArch64 processors in general-purpose
computing, securing software running on AArch64 systems against control-flow
hijacking attacks has become a critical part toward secure computation. Shadow
stacks keep shadow copies of function return addresses and, when protected from
illegal modifications and coupled with forward-edge control-flow integrity,
form an effective and proven defense against such attacks. However, AArch64
lacks native support for write-protected shadow stacks, while software
alternatives either incur prohibitive performance overhead or provide weak
security guarantees.

We present *InversOS*, the first hardware-assisted write-protected shadow
stacks for AArch64 user-space applications, utilizing commonly available
features of AArch64 to achieve efficient intra-address space isolation (called
*Privilege Inversion*) required to protect shadow stacks. Privilege Inversion
adopts unconventional design choices that run protected applications in the
kernel mode and mark operating system (OS) kernel memory as user-accessible;
InversOS therefore uses a novel combination of OS kernel modifications,
compiler transformations, and another AArch64 feature to ensure the safety of
doing so and to support legacy applications. We show that InversOS is secure by
design, effective against various control-flow hijacking attacks, and
performant on selected benchmarks and applications (incurring overhead of 7.0%
on LMBench, 7.1% on SPEC CPU 2017, and 3.0% on Nginx web server).
