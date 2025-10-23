---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

<ul>
{% assign items = site.projects | sort: "date" | reverse %}
{% for item in items %}
  <li>
    <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
    {% if item.excerpt %} — {{ item.excerpt }}{% endif %}
    {% if item.paperurl %} — <a href="{{ item.paperurl }}">PDF</a>{% endif %}
  </li>
{% endfor %}
</ul>


