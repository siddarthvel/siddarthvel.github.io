---
layout: default
title: Projects
---

# Projects

<ul style="list-style:none; padding-left:0;">
  {% for p in site.projects %}
    <li style="margin: 20px 0;">
      <h2 style="margin-bottom:6px;"><a href="{{ p.url }}">{{ p.title }}</a></h2>
      {% if p.summary %}<p style="margin:0;">{{ p.summary }}</p>{% endif %}
      {% if p.tags %}
        <p style="margin:6px 0 0 0; font-size: 0.9em;">
          {% for t in p.tags %}<span style="margin-right:8px;">#{{ t }}</span>{% endfor %}
        </p>
      {% endif %}
    </li>
  {% endfor %}
</ul>
