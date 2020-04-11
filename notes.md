---
layout: default
title: 碎碎念
---
{% for note in site.notes reversed %}
<div class="box" id="date-{{ note.date | date: "%Y-%m-%d %H:%M" }}">
  <div class="date">
    <date>
    <a href="#date-{{ note.date | date: "%Y-%m-%d %H:%M" }}">{{ note.date | date: "%Y-%m-%d %H:%M"}}</a>
    </date>
  </div>
  {{ note.content | markdownify }}
</div>
{% endfor %}
