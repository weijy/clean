---
layout: default
title: 碎碎念
---
{% for note in site.notes reversed %}
<div class="card" id="date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">
  <div class="date">
    <date>
    <a href="#date-{{ note.date | date: "%Y-%m-%d %H:%M" }}{{ note.slug }}">{{ note.date | date: "%Y-%m-%d %H:%M"}}</a>
    </date>
  </div>
  {{ note.content | markdownify }}
</div>
{% endfor %}
