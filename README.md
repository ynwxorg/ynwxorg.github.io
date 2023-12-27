书籍是人类进步的阶梯

{% for file in site.static_files %}
    {% if file.path contains '.' %}
[{{ file.name | remove: 'index.html' | remove: '.md'}}]({{ file.path | absolute_url | remove: '.md'}})
    {% endif %}
{% endfor %}