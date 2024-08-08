---
collection: publications
title: "Enforcing Low-Cost Security for ARM"
permalink: /publication/2023-09-09-PhD-Dissertation
link: "http://hdl.handle.net/1802/37786"
classes: wide
bibtex:
  type: phdthesis
  id: Shen@UR
  author:
    - Shen, Zhuojia
  title: "Enforcing Low-Cost Security for {ARM}"
  school: "University of Rochester"
  isbn: "9798380310833"
  url: "http://hdl.handle.net/1802/37786"
date: "2023-09-09"
pdf: "/assets/files/Shen@UR.pdf"
---

A great share of today's computer systems, including most embedded and
microcontroller (MCU) systems and an increasing number of desktops and servers,
run a processor based on ARM architectures.  Securing these systems against
runtime attacks that exploit common software vulnerabilities poses great
challenges; effective mitigations usually incur prohibitive overhead, while
practical defenses typically only provide less-than-ideal security guarantees.

This dissertation makes four contributions to low-cost security policy
enforcement for ARM-based systems.  First, we develop a novel compiler-based
intra-address space isolation technique and use it to efficiently enforce
return address integrity for bare-metal embedded applications running on
ARM-based MCUs.  Second, we leverage ARM's hardware debugging facilities to
enforce execute-only memory with negligible overhead.  Third, utilizing the
execute-only memory we developed and combining compiler- and hardware-based
techniques, we measurably strengthen layout randomization defenses on ARM-based
MCUs to effectively and efficiently resist leakage-equipped attacks and their
brute force variants.  Lastly, we extend hardware-assisted write-protected
shadow stacks to AArch64 (64-bit ARM) user-space applications, using a novel
combination of commonly available AArch64 hardware features, operating system
kernel modifications, and compiler transformations.
