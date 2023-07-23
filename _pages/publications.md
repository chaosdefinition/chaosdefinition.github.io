---
layout: single
author_profile: true
title: Publications
permalink: /publications
classes: wide
---

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
