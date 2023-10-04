---
layout: single
author_profile: true
permalink: /
redirect_from:
  - /about
  - /about.html
classes: wide
---

Hello there!

I am Zhuojia Shen (沈卓佳),
a Software Engineer at Apple.
I obtained my PhD from the
[Department of Computer Science](https://www.cs.rochester.edu)
at the [University of Rochester](https://www.rochester.edu),
where I was advised by
[Prof. John Criswell](https://www.cs.rochester.edu/u/criswell).
Before that,
I got my Bachelor's degree in [School of Computer Science](http://cs.bit.edu.cn)
at [Beijing Institute of Technology](http://www.bit.edu.cn).

## Research Interests

I work on the broad area of computer systems security.
My current research interests lie in
**low-cost security enforcement on ARM systems**,
using novel combinations of hardware and architectural features as well as
operating system and compiler techniques.
I also had experience developing novel software-based defenses against
side-channel attacks.

{{ author.name }}

## Publications

{% for post in site.publications reversed %}
 1. <p>
    {% for autr in post.bibtex.author %}
      {% assign aut = autr | split: ", " | reverse | join: " " %}
      {% if forloop.length > 1 and forloop.last %} and {% endif %}
      {% if aut == site.author.name %}<b>{{ aut }}</b>{% else %}{{ aut }}{% endif %}{% if forloop.last %}.{% elsif forloop.length > 2 %},{% endif %}
    {% endfor %}
    <a href="{{ post.bibtex.url }}" target="_blank">{{ post.title }}</a>.
    {% case post.bibtex.type %}
      {% when 'inproceedings' %}
        In <i>{{ post.bibtex.booktitle }}</i>{% if post.bibtex.series %} ({{ post.bibtex.series }}){% endif %}.
      {% when 'phdthesis' %}
        <i>Ph.D. Dissertation</i>.
      {% else %}
        <i>{{ post.bibtex.journal }}</i>.
    {% endcase %}
    {% if post.bibtex.location %}
      {{ post.bibtex.location }}.
    {% elsif post.bibtex.address %}
      {{ post.bibtex.address }}.
    {% elsif post.bibtex.school %}
      {{ post.bibtex.school }}.
    {% endif %}
    {{ post.date | date: "%B %Y" }}.
    </p>
{% endfor %}
