---
layout: page
title: About
description: 面向百度编程
keywords: xiangxiwei, 向希为
comments: true
menu: 关于
permalink: /about/
---

万物孕而不相害，道并行而不相悖

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
