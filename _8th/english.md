---
title: "8th Grade English"
permalink: /8th/english/
layout: single
---

<div class="page-with-sidebar" style="display:flex; flex-wrap:nowrap;">

<!-- Left sidebar -->
{% include sidebar-grades.html %}

<!-- Main content -->
<div style="flex:1; padding-left:10px;">

## Assignments

{% assign english_posts = site.posts | where: "grade", 8 | where: "subject", "english" | sort: "assignment_number" %}

{% for post in english_posts %}
- **Assignment {{ post.assignment_number }}:** [{{ post.title }}]({{ post.url }})
{% endfor %}

</div>
</div>
