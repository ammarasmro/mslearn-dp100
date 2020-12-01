---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

{% assign labs = site.pages | where_exp:"page", "page.url contains '/instructions'" %}
| Hyperlinks to each of the lab exercises listed below. |
| ------- | 
{% for activity in labs  %}| [{{ activity.lab.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
