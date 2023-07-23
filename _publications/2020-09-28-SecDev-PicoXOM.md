---
collection: publications
title: "Fast Execute-Only Memory for Embedded Systems"
permalink: /publication/2020-09-28-SecDev-PicoXOM
link: "https://doi.org/10.1109/SecDev45635.2020.00017"
classes: wide
bibtex:
  type: inproceedings
  id: PicoXOM@SecDev20
  author:
    - Shen, Zhuojia
    - Dharsee, Komail
    - Criswell, John
  title: "Fast Execute-Only Memory for Embedded Systems"
  booktitle: "Proceedings of the 2020 IEEE Secure Development Conference"
  series: "SecDev '20"
  isbn: "978-1-7281-8388-6"
  location: "Atlanta, GA, USA"
  pages: "7--14"
  numpages: "8"
  url: "https://doi.org/10.1109/SecDev45635.2020.00017"
  doi: "10.1109/SecDev45635.2020.00017"
  publisher: "IEEE Computer Society"
  address: "Washington, DC, USA"
date: "2020-09-28"
pdf: "/assets/files/PicoXOM@SecDev20.pdf"
repository: "https://github.com/URSec/PicoXOM"
---

Remote code disclosure attacks threaten embedded systems as they allow
attackers to steal intellectual property or to find reusable code for use in
control-flow hijacking attacks. Execute-only memory (XOM) prevents remote code
disclosures, but existing XOM solutions either require a memory management unit
that is not available on ARM embedded systems or incur significant overhead.

We present *PicoXOM*: a fast and novel XOM system for ARMv7-M and ARMv8-M
devices which leverages ARM's Data Watchpoint and Tracing unit along with the
processor's simplified memory protection hardware. On average, PicoXOM incurs
0.33% performance overhead and 5.89% code size overhead on two benchmark suites
and five real-world applications.
