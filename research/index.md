---
layout: default
title: Research
---

# Research Posters & Projects

{% assign sorted_research = site.research | sort: 'order' %}
{% for r in sorted_research %}
- **[{{ r.title }}]({{ r.url | relative_url }})**
{% endfor %}
