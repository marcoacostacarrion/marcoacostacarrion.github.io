---
title: "Research"
permalink: /publications/
layout: archive
author_profile: true
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
