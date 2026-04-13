# Downloads

These are the current releases stored in the `releases/` folder.

---

## Available Files

{% for file in site.static_files %}
  {% if file.path contains '/releases/' %}
- [{{ file.name }}]({{ file.path }})
  {% endif %}
{% endfor %}
