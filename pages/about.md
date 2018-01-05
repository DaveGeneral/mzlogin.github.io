---
layout: page
title: About
description: IRlab 信息检索实验室博客
keywords: SDU，IRLab
comments: true
menu: 关于
permalink: /about/
---

山东大学信息检索实验室成立于2004年，是一个年轻、富有朝气的研究团队。
实验室在博士生导师马军教授的带领下，逐渐发展壮大，形成了稳定的研究方向梯队，
并在国内信息检索、多媒体计算、大数据处理、社会计算、健康计算、
自然语言处理等领域具有了较高的知名度。

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
