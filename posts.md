---
layout: page
image: https://cn.bing.com/th?id=OHR.SaltonSea_ZH-CN1265210111_1920x1080.jpg&rf=LaDigue_1920x1080.jpg
title: 短话长说
title-hide: true
---

<ul>
        {% for post in site.posts %}
        <li>
            <span>{{ post.date | date: '%Y/%m/%d' }}</span>
            
            <a href="{{ post.url | relative_url}}">{{ post.title }}</a>
        </li>
        {% endfor %}
</ul>
