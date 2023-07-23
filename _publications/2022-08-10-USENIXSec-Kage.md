---
collection: publications
title: "Holistic Control-Flow Protection on Real-Time Embedded Systems with Kage"
permalink: /publication/2022-08-10-USENIXSec-Kage
link: "https://www.usenix.org/conference/usenixsecurity22/presentation/du"
classes: wide
bibtex:
  type: inproceedings
  id: Kage@UsenixSec22
  author:
    - Du, Yufei
    - Shen, Zhuojia
    - Dharsee, Komail
    - Zhou, Jie
    - Walls, Robert J.
    - Criswell, John
  title: "Holistic Control-Flow Protection on Real-Time Embedded Systems with {Kage}"
  booktitle: "Proceedings of the 31st USENIX Security Symposium"
  series: "Security '22"
  isbn: "978-1-939133-31-1"
  location: "Boston, MA, USA"
  pages: "2281--2298"
  url: "https://www.usenix.org/conference/usenixsecurity22/presentation/du"
  publisher: "USENIX Association"
  address: "Berkeley, CA, USA"
date: "2022-08-10"
pdf: "/assets/files/Kage@UsenixSec22.pdf"
repository: "https://github.com/URSec/Kage"
---

This paper presents *Kage*: a system that protects the control data of both
application and kernel code on microcontroller-based embedded systems. Kage
consists of a Kage-compliant embedded OS that stores all control data in
separate memory regions from untrusted data, a compiler that transforms code to
protect these memory regions efficiently and to add forward-edge control-flow
integrity checks, and a secure API that allows safe updates to the protected
data. We implemented Kage as an extension to FreeRTOS, an embedded real-time
operating system. We evaluated Kage's performance using the CoreMark benchmark.
Kage incurred a 5.2% average runtime overhead and 49.8% code size overhead.
Furthermore, the code size overhead was only 14.2% when compared to baseline
FreeRTOS with the MPU enabled. We also evaluated Kage's security guarantees by
measuring and analyzing reachable code-reuse gadgets. Compared to FreeRTOS,
Kage reduces the number of reachable gadgets from 2,276 to 27, and the
remaining 27 gadgets cannot be stitched together to launch a practical attack.
