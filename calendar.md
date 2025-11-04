---
layout: page
title: 🏠 Home
description: Listing of course modules and topics.
nav_order: 1
permalink: /
---

# **Data 8: Foundations of Data Science**

{: .mb-2 }
UC Berkeley, Fall 2025
{: .mb-2 .fs-6}

[Ed](https://edstem.org/us/courses/83132/discussion){: .btn .btn-ed}
[Pensieve](https://www.pensieve.co/student/classes/data8_fa25/my-assignments){: .btn .btn-pensieve}
[Zoom](https://berkeley.zoom.us/j/99133083020){: .btn .btn-zoom}
[Lecture Recordings](https://bcourses.berkeley.edu/courses/1547037/external_tools/90481){: .btn .btn-bcourses}
[Office Hours Queue](https://oh.data8.org/){: .btn .btn-officehours}
[Extensions](https://forms.gle/8bC3hu2334NY3EHe9){: .btn .btn-extensions}
[Jump to Current Week](https://www.data8.org/fa25/#week-{{site.current_week}}){: .btn .btn-currweek}

{% include announcements-navigation.html %}

{% assign mods = site.modules | where: 'class', 'Berkeley' %}
{% assign active-mods = '' | split: '' %}

{% for mod in mods %}
{% if mod.status == 'Active' %}
{% assign active-mods = active-mods | push: mod %}
{% endif %}
{% endfor %}

{% for module in active-mods %}
{{ module }}
{% endfor %}

<script src="{{ '/assets/scripts/announcement-navigation.js' | relative_url }}"></script>
