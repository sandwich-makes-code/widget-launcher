#  Downloads
---
layout: default
title: Downloads
---

# Downloads

These are the current releases stored in the `releases/` folder.

> Click any file name below to download it.

---

## Available Files

<ul>
{% for file in site.static_files %}
  {% if file.path contains '/releases/' %}
    <li>
      <a href="{{ file.path | relative_url }}">{{ file.name }}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>
