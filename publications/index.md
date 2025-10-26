---
layout: default
title: Publications
---

# Publications

{% for pub in site.publications %}
- **[{{ pub.title }}]({{ pub.url | relative_url }})**  
  {{ pub.authors }}  
  *{{ pub.venue }}, {{ pub.year }}*
{% endfor %}
