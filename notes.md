---
layout: default
permalink: /notes/
---

## My notes

{% for tag in site.tags %}
  {% if tag[0] == "notes" %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
  {% endif %}
{% endfor %}
