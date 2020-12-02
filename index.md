---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Azure Machine Learning Exercises

This repository contains the hands-on lab exercises for Microsoft course [DP-100 *Designing and Implementing a Data Science Solution on Azure*](https://docs.microsoft.com/learn/certifications/courses/dp-100t01) and the equivalent [self-paced modules on Microsoft Learn](https://docs.microsoft.com/learn/paths/build-ai-solutions-with-azure-ml-service/). The exercises are designed to accompany the learning materials and enable you to practice using the technologies they describe.

To complete these exercises, you'll require a Microsoft Azure subscription. If your instructor has not provided you with one, you can sign up for a free trial at [https://azure.microsoft.com](https://azure.microsoft.com).

{% assign labs = site.pages | where_exp:"page", "page.url contains '/instructions'" %}
| Exercises |
| ------- | 
{% for activity in labs  %}| [{{ activity.lab.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
