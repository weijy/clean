---
layout: default
title: 碎碎念
---
{% for note in site.notes %}
<div class="card" id="date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">
  <small><date>
    <a href="#date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">{{ note.date | date: "%Y-%m-%d %H:%M"}}</a>
    </small></date>
  {{ note.content | markdownify }}
</div>
{% endfor %}
