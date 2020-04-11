---
layout: default
---
![卓别林与海伦凯勒](/clean/images/zhuobielin_hailunkaile.jgp)
<blockquote>{{ site.summer }}</blockquote>
<hr >
{% assign notes = site.notes | reverse %}

<div class="box">
  <div class="box-heading">
    # 最近的碎碎念 {{ note.date | date: "%Y-%m-%d"}}
  </div>
  {{ notes[0].content | markdownify }}
</div>
