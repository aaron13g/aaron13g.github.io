---
layout: page
title: Academic Projects
subtitle: Selected evaluation and systems design work
---

{% assign items = site.academic_projects %}
{% if items %}
  {% for p in items %}
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
