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

## Work in Progress
{% for post in site.publications %}
  {% if post.type == "work" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
