---
collection: publications
title: "Silhouette: Efficient Protected Shadow Stacks for Embedded Systems"
permalink: /publication/2020-08-12-USENIXSec-Silhouette
link: "https://www.usenix.org/conference/usenixsecurity20/presentation/zhou-jie"
classes: wide
bibtex:
  type: inproceedings
  id: Silhouette@UsenixSec20
  author:
    - Zhou, Jie
    - Du, Yufei
    - Shen, Zhuojia
    - Ma, Lele
    - Criswell, John
    - Walls, Robert J.
  title: "Silhouette: Efficient Protected Shadow Stacks for Embedded Systems"
  booktitle: "Proceedings of the 29th USENIX Security Symposium"
  series: "Security '20"
  isbn: "978-1-939133-17-5"
  location: "Boston, MA, USA"
  pages: "1219--1236"
  url: "https://www.usenix.org/conference/usenixsecurity20/presentation/zhou-jie"
  publisher: "USENIX Association"
  address: "Berkeley, CA, USA"
date: "2020-08-12"
pdf: "/assets/files/Silhouette@UsenixSec20.pdf"
repository: "https://github.com/URSec/Silhouette"
---

Microcontroller-based embedded systems are increasingly used for applications
that can have serious and immediate consequences if compromised—including
automobile control systems, smart locks, drones, and implantable medical
devices. Due to resource and execution-time constraints, C is the primary
language used for programming these devices. Unfortunately, C is neither
type-safe nor memory-safe, and control-flow hijacking remains a prevalent
threat.

This paper presents *Silhouette*: a compiler-based defense that efficiently
guarantees the integrity of return addresses, significantly reducing the attack
surface for control-flow hijacking. Silhouette combines an incorruptible shadow
stack for return addresses with checks on forward control flow and memory
protection to ensure that all functions return to the correct dynamic caller.
To protect its shadow stack, Silhouette uses *store hardening*, an efficient
intra-address space isolation technique targeting various ARM architectures
that leverages special store instructions found on ARM processors.

We implemented Silhouette for the ARMv7-M architecture, but our techniques are
applicable to other common embedded ARM architectures. Our evaluation shows
that Silhouette incurs a geometric mean of 1.3% and 3.4% performance overhead
on two benchmark suites. Furthermore, we prototyped *Silhouette-Invert*, an
alternative implementation of Silhouette, which incurs just 0.3% and 1.9%
performance overhead, at the cost of a minor hardware change.
