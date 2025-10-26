---
layout: default
title: Research
---

# Research Posters & Projects

{% for r in site.research %}
- **[{{ r.title }}]({{ r.url | relative_url }})**
{% endfor %}
