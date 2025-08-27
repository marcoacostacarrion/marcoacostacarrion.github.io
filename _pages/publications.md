---
layout: splash
title: "Marco Acosta"
permalink: /publications/
author_profile: true
header:
  overlay_image: /images/ProfilePicture2.jpg
  overlay_filter: 0.25 # darkens the image so text is readable (0–1)
---




## JMP
{% assign jmps = site.publications | where: "type", "JMP" | sort: "date" | reverse %}
{% for post in jmps %}
  {% include archive-single-jmp.html post=post %}
{% endfor %}

## Working Papers
{% assign works = site.publications | where: "type", "work" | sort: "date" | reverse %}
{% for post in works %}
  {% include archive-single-work.html post=post %}
{% endfor %}

## Publications
{% for post in site.publications %}
  {% if post.type == "publications" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}



## Work in Progress

- **Welfare Impact from Merit Based to Lottery School Assignment: Evidence from Mexico City High School Matching Reform**




