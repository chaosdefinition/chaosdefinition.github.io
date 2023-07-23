---
collection: publications
title: "Shielding Software from Privileged Side-Channel Attacks"
permalink: /publication/2018-08-15-USENIXSec-Apparition
link: "https://www.usenix.org/conference/usenixsecurity18/presentation/dong"
classes: wide
bibtex:
  type: inproceedings
  id: Apparition@UsenixSec18
  author:
    - Dong, Xiaowan
    - Shen, Zhuojia
    - Criswell, John
    - Cox, Alan L.
    - Dwarkadas, Sandhya
  title: "Shielding Software from Privileged Side-Channel Attacks"
  booktitle: "Proceedings of the 27th USENIX Security Symposium"
  series: "Security '18"
  isbn: "978-1-939133-04-5"
  location: "Baltimore, MD, USA"
  pages: "1441--1458"
  numpages: "18"
  url: "https://www.usenix.org/conference/usenixsecurity18/presentation/dong"
  publisher: "USENIX Association"
  address: "Berkeley, CA, USA"
date: "2018-08-15"
pdf: "/assets/files/Apparition@UsenixSec18.pdf"
---

Commodity operating system (OS) kernels, such as Windows, Mac OS X, Linux, and
FreeBSD, are susceptible to numerous security vulnerabilities. Their monolithic
design gives successful attackers complete access to all application data and
system resources. Shielding systems such as InkTag, Haven, and Virtual Ghost
protect sensitive application data from compromised OS kernels. However, such
systems are still vulnerable to side-channel attacks. Worse yet, compromised OS
kernels can leverage their control over privileged hardware state to exacerbate
existing side channels; recent work has shown that a compromised OS kernel can
steal entire documents via side channels.

This paper presents defenses against page table and last-level cache (LLC)
side-channel attacks launched by a compromised OS kernel. Our page table
defenses restrict the OS kernel's ability to read and write page table pages
and defend against page allocation attacks, and our LLC defenses utilize the
Intel Cache Allocation Technology along with memory isolation primitives. We
prototype our solution in a system we call Apparition, building on an optimized
version of Virtual Ghost. Our evaluation shows that our side-channel defenses
add 1% to 18% (with up to 86% for one application) overhead to the optimized
Virtual Ghost (relative to the native kernel) on real-world applications.
