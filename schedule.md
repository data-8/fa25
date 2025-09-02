---
layout: page
title: 🏢 Weekly Calendar & OH
description: The weekly event schedule.
nav_order: 2
---

# **Weekly Calendar & Office Hours**

We use an [online sign-up system](https://oh.data8.org/) to help keep track of everyone.

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}
