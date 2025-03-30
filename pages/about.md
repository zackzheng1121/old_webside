---
layout: page
title: About
description: 只是一個會c#的貓
keywords: Zackzheng
comments: true
menu: 關於我
permalink: /about/
---

我是zackzheng，一個學生，目前會一點C#，其他的語言則在持續努力學習中!

## 聯繫我

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
