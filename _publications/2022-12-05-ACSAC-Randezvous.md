---
collection: publications
title: "Randezvous: Making Randomization Effective on MCUs"
permalink: /publication/2022-12-05-ACSAC-Randezvous
link: "https://doi.org/10.1145/3564625.3567970"
classes: wide
bibtex:
  type: inproceedings
  id: Randezvous@ACSAC22
  author:
    - Shen, Zhuojia
    - Dharsee, Komail
    - Criswell, John
  title: "Randezvous: Making Randomization Effective on {MCUs}"
  booktitle: "Proceedings of the 38th Annual Computer Security Applications Conference"
  series: "ACSAC '22"
  isbn: "978-1-4503-9759-9"
  location: "Austin, TX, USA"
  pages: "28--41"
  numpages: "14"
  url: "https://doi.org/10.1145/3564625.3567970"
  doi: "10.1145/3564625.3567970"
  publisher: "ACM"
  address: "New York, NY, USA"
date: "2022-12-05"
pdf: "/assets/files/Randezvous@ACSAC22.pdf"
repository: "https://github.com/URSec/Randezvous"
---

Internet-of-Things devices such as autonomous vehicular sensors, medical
devices, and industrial cyber-physical systems commonly rely on small,
resource-constrained microcontrollers (MCUs). MCU software is typically written
in C and is prone to memory safety vulnerabilities that are exploitable by
remote attackers to launch code reuse attacks and code/control data leakage
attacks.

We present *Randezvous*, a highly performant diversification-based mitigation
to such attacks and their brute force variants on ARM MCUs. Atop code/data
layout randomization and an efficient execute-only code approach, Randezvous
creates decoy pointers to camouflage control data in memory; code pointers in
the stack are then protected by a diversified shadow stack, local-to-global
variable promotion, and return address nullification. Moreover, Randezvous adds
a novel delayed reboot mechanism to slow down persistent attacks and mitigates
control data spraying attacks via global guards. We demonstrate Randezvous’s
security by statistically modeling leakage-equipped brute force attacks under
Randezvous, crafting a proof-of-concept exploit that shows Randezvous’s
efficacy, and studying a real-world CVE. Our evaluation of Randezvous shows low
overhead on three benchmark suites and two applications.
