---
collection: publications
title: "Spectres, Virtual Ghosts, and Hardware Support"
permalink: /publication/2018-06-02-HASP-SpectreVG
link: "https://doi.org/10.1145/3214292.3214297"
classes: wide
bibtex:
  type: inproceedings
  id: SpectreVG@HASP18
  author:
    - Dong, Xiaowan
    - Shen, Zhuojia
    - Criswell, John
    - Cox, Alan
    - Dwarkadas, Sandhya
  title: "Spectres, {Virtual Ghosts}, and Hardware Support"
  booktitle: "Proceedings of the 7th International Workshop on Hardware and Architectural Support for Security and Privacy"
  series: "HASP '18"
  isbn: "978-1-4503-6500-0"
  location: "Los Angeles, CA, USA"
  pages: "5:1--5:9"
  articleno: "5"
  numpages: "9"
  url: "https://doi.org/10.1145/3214292.3214297"
  doi: "10.1145/3214292.3214297"
  publisher: "ACM"
  address: "New York, NY, USA"
date: "2018-06-02"
pdf: "/assets/files/SpectreVG@HASP18.pdf"
---

Side-channel attacks, such as Spectre and Meltdown, that leverage speculative
execution pose a serious threat to computing systems. Worse yet, such attacks
can be perpetrated by compromised operating system (OS) kernels to bypass
defenses that protect applications from the OS kernel.

This work evaluates the performance impact of three different defenses against
in-kernel speculation side-channel attacks within the context of Virtual Ghost,
a system that protects user data from compromised OS kernels: Intel MPX bounds
checks, which require a memory fence; address bit-masking and testing, which
creates a dependence between the bounds check and the load/store; and the use
of separate virtual address spaces for applications, the OS kernel, and the
Virtual Ghost virtual machine, forcing a speculation boundary. Our results
indicate that an instrumentation-based bit-masking approach to protection
incurs the least overhead by minimizing speculation boundaries. Our work also
highlights possible improvements to Intel MPX that could help mitigate
speculation side-channel attacks at a lower cost.
