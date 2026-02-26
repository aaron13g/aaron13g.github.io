---
layout: page
title: Academic Projects
subtitle: Selected evaluation and systems design work
---

{% assign items = site.academic_projects %}
{% if items and items.size > 0 %}
  {% assign sorted = items | sort: "order" %}
  {% for p in sorted %}
### [{{ p.short_title | default: p.title }}]({{ p.url }})

{% if p.summary %}
{{ p.summary }}
{% else %}
{{ p.excerpt | strip_html | truncate: 220 }}
{% endif %}

---
  {% endfor %}
{% else %}
No academic projects yet.
{% endif %}
