{% for file in site.static_files %}{% if file.path contains 'book/' %}

[{{ file.name | remove: 'index.html' | remove: '.md'}}]({{ file.path | absolute_url | remove: '.md'}})

{% endif %}{% endfor %}