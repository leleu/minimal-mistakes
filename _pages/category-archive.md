---
title: "Things We've Written"
layout: categories
permalink: /articles/
author_profile: true
---
{% for post in site.categories.articles %}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}