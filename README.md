---
layout: default
title: Directory Listing
markdown: kramdown
---

# Files in This Directory:

{% for file in site.static_files %}
  {% if file.path contains '.' %}
    - [{{ file.name | remove: 'index.html' }}]({{ file.path | absolute_url }})
  {% endif %}
{% endfor %}
