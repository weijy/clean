---
layout: default
title: 碎碎念
---
{% for note in site.notes reversed %}

<div class="box">
  <div class="box-heading">
    # {{ note.date | date: "%Y-%m-%d %H:%M"}}
  </div>
  {{ note.content | markdownify }}
</div>
{% endfor %}
