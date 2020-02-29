---
layout: page
title: About
description: 绝对不要看 眼睛里的郁金香
keywords: Zhuang Ma, 马壮
comments: true
menu: 关于
permalink: /about/
---

不要有趣 要有用

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
