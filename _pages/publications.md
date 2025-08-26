---
title: ""
permalink: /publications/
layout: archive
author_profile: true
---

## JMP
{% assign jmps = site.publications | where: "type", "JMP" | sort: "date" | reverse %}
{% for post in jmps %}
  {% include archive-single-jmp.html post=post %}
{% endfor %}

---
## Publications
{% for post in site.publications %}
  {% if post.type == "publications" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

---

## Working in Papers
{% for post in site.publications %}
  {% if post.type == "working" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
