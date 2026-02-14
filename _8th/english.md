---
title: "8th Grade English"
permalink: /8th/english/
layout: single
sidebar:
  include: sidebar-grades.html
---

## Assignments

{% assign english_posts = site.posts | where: "grade", 8 | where: "subject", "english" | sort: "assignment_number" %}

{% for post in english_posts %}
- **Assignment {{ post.assignment_number }}:**  
  [{{ post.title }}]({{ post.url }})
{% endfor %}
