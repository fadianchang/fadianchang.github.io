---
layout: page
title: Links
description: 链接
keywords: 友情链接
comments: true
menu: 链接
permalink: /links/
---

> 三人行 必有我师

{% for link in site.data.links %}
  {% if link.src == 'life' %}
* [{{ link.name }}]({{ link.url }})
  {% endif %}
{% endfor %}

> 友情链接

{% for link in site.data.links %}
  {% if link.src == 'www' %}
* [{{ link.name }}]({{ link.url }})
  {% endif %}
{% endfor %}
