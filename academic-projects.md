---
layout: page
title: Academic Projects
subtitle: Selected evaluation and systems design work
---

{% assign sorted = site.academic_projects | sort: "order" %}

{% for project in sorted %}
### [{{ project.short_title }}]({{ project.url }})

{{ project.excerpt }}

---

{% endfor %}
