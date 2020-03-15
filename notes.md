---
layout: default
title: 碎碎念
---
{% for note in site.data.notes %}
<div class="card" id="date-{{ note.date | date: "%Y-%m-%d" }}{{ note.slug }}">
  <h2 class="date">
    <a href="#date-{{ note.date | date: "%Y-%m-%d" }}{{ note.slug }}">{{ note.date | date: "%Y-%m-%d" }} #</a>
  </h2>
  {{ note.content | markdownify }}
</div>
{% endfor %}
