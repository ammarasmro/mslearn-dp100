---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Hyperlinks to each of the lab exercises listed below.

## Exercises

{% assign labs = site.pages | where_exp:"page", "page.url contains '/instructions'" %}
| Exercise |
| ------- | 
{% for activity in labs  %}| [{{ activity.lab.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
