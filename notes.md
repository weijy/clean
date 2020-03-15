---
layout: default
title: 碎碎念
---
{% for note in site.notes %}
<div class="card" id="date-{{ note.date | date: "%Y-%m-%d" }}{{ note.slug }}">
  <date>
    <a href="#date-{{ note.date | date: "%Y-%m-%d" }}{{ note.slug }}">{{ note.date }} #</a>
  </date>
  {{ note.content | markdownify }}
</div>
{% endfor %}
