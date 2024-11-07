---
title: "dispatch"
layout: archive
permalink: /dispatch
---

{% assign posts = site.categories.dispatch %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}