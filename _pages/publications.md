---
title: ""
permalink: /publications/
layout: archive
author_profile: true
---

## JMP
{% for post in site.publications %}
  {% if post.type == "JMP" %}
    {% include archive-single.html %}
  {% endif %}
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
