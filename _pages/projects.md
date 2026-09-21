---
layout: page
title: photos
permalink: /photos/
description: Photos and short notes from conference talks and other research events.
nav: true
nav_order: 3
display_categories: []
horizontal: false
---

<!-- pages/projects.md -->
<!-- Each entry in _projects/ is one talk/event: a photo, a one-line description, -->
<!-- and (optionally) a longer note on its own page. See _projects/README.md for how to add one. -->
<div class="projects">
{% assign sorted_projects = site.projects | sort: "importance" %}
<div class="row row-cols-1 row-cols-md-3">
  {% for project in sorted_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>
</div>
