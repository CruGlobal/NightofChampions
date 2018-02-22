---
title: Hall of Faith Inductees
date: 2017-11-13 14:51:00 Z
permalink: "/inductees/"
position: 1
description: 
---

{% for post in site.inductees %}
<div class="col-xs-12 col-sm-6">
<div class="team-entry">
<a class="team-img" href="{{ post.url | replace: '.html', '' }}"><img class="img-responsive" src="{{ post.img }}" alt=""></a>
<a class="team-title" href="{{ post.url | replace: '.html', '' }}">{{ post.title }}</a>
<a class="team-pos">{{ post.year }}</a>
<div class="team-text">{{ post.content | strip_html | truncate: 200, '...' }}</div>
</div>
</div>
{% endfor %}
