---
title: ""
permalink: /publications/
layout: archive
#author_profile: true
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

## Working Papers
{% assign works = site.publications | where: "type", "work" | sort: "date" | reverse %}
{% for post in works %}
  {% include archive-single-work.html post=post %}
{% endfor %}




