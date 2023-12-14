---
layout: single
author_profile: true
title: Curriculum Vitae
permalink: /cv
classes: wide
date: "2023-12-13"
---

## Education

- **University of Rochester**, Rochester, NY, USA \\
  Ph.D. in Computer Science, Sept. 2016 -- June 2023 \\
  *Advisor*: Prof. John Criswell \\
  *Thesis*: Enforcing Low-Cost Security for ARM
- **University of Rochester**, Rochester, NY, USA \\
  M.S. in Computer Science, Sept. 2016 -- Jan. 2019
- **Beijing Institute of Technology**, Beijing, China \\
  B.S. in Computer Science & Technology, Sept. 2012 -- June 2016

## Work Experience

- **Apple**, Cupertino, CA, USA \\
  Software Engineer, Aug. 2023 -- Present
- **VMware**, ~~Palo Alto, CA, USA~~ (Remote) \\
  Intern - Member of Technical Staff - VM Monitor, June 2020 -- Aug. 2020 \\
  *Mentor*: Dr. Zheng Cui \\
  - Designed and implemented a live patch generation tool for VMKernel
  - Implemented a live patch applying mechanism to verify patch correctness
- **VMware**, Boston, MA, USA \\
  Intern - Member of Technical Staff - VM Monitor, May 2019 -- Aug. 2019 \\
  *Mentor*: Dr. Jiajun Cao \\
  - Designed and implemented a generic interface for sharing
    Page-Modification Logging (PML), an Intel processor feature, among modules
    in the VM monitor
  - Evaluated the performance of vMotion utilizing the PML interface
- **Taoxue Information Technology Co., Ltd**, Beijing, China \\
  Co-Founder & CTO (part-time), May 2014 -- Feb. 2015 \\
  - Member of Taoxue Backend Team, main developer and maintainer of
    Taoxue web server
  - Provided technical support to Taoxue iOS and Android Client Teams

## Skills

- Programming languages: C/C++, Java, C#, Bash, Python, Ruby, JavaScript,
                         x86/ARM/PowerPC/MIPS Assembly, SQL
- Software & tools: Vim, Git, LLVM, Docker, Mutt, Eclipse, Sublime Text,
                    Microsoft Office, LaTeX, Xcode
- Platforms: Linux, Windows, macOS, FreeBSD, VMware ESXi

## Research Interests

- Systems: Operating Systems, Compiler Transformations
- Security: Operating System Security, Embedded System Security, Memory Safety,
            Control-Flow Integrity, Compiler Transformations for Security

## Publications

{% for post in site.publications reversed %}
 1. <p>
    <b>{{ post.title }}</b>.
    {% case post.bibtex.type %}
      {% when 'inproceedings' %}
        In <i>{{ post.bibtex.series }}</i>.
      {% when 'phdthesis' %}
        <i>Ph.D. Dissertation</i>.
      {% else %}
        <i>{{ post.bibtex.journal }}</i>.
    {% endcase %}
    </p>
{% endfor %}

## Teaching Experience

- **University of Rochester**, Rochester, NY, USA \\
  Graduate Teaching Assistant, Sept. 2018 -- Dec. 2018 \\
  *Course*: CSC 256/456 Operating Systems \\
  *Instructor*: Prof. Sandhya Dwarkadas
- **University of Rochester**, Rochester, NY, USA \\
  Graduate Teaching Assistant, Jan. 2018 -- May 2018 \\
  *Course*: CSC 261/461 Database Systems \\
  *Instructor*: Dr. Tamal Biswas
- **University of Rochester**, Rochester, NY, USA \\
  Graduate Teaching Assistant, Sept. 2017 -- Dec. 2017 \\
  *Course*: CSC 256/456 Operating Systems \\
  *Instructor*: Prof. John Criswell
- **Beijing Institute of Technology**, Beijing, China \\
  Undergraduate Teaching Assistant, Mar. 2016 -- June 2016 \\
  *Course*: Computational Theory & Algorithm Analysis Design \\
  *Course*: Combinatorial Mathematics \\
  *Instructor*: Prof. Qinghui Liu

## Honors & Awards

- Senior honors thesis,
  Beijing Institute of Technology, 2016
- Third-class People’s Scholarship (four times),
  Beijing Institute of Technology, 2012 -- 2015
