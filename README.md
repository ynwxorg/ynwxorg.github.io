[滕王阁序](twgx.md)
[道德经](ddj.md)
[前出师表](qcsb.md)
{% for file in site.static_files %}
  {% if file.path contains '.' %}
    - [{{ file.name }}]({{ file.path }})
  {% endif %}
{% endfor %}