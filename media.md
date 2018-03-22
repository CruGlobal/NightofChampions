---
title: Media
description: Press Releases
date: 2017-11-13 14:53:00 Z
position: 5
permalink: /media/
layout: media
---

{% for post in site.posts %}
<div class="col-xs-12 col-sm-12">
<div class="team-entry">
<a class="team-title" style="text-decoration: underline; width: 100%;" href="{{ post.url | replace: '.html', '' }}">{{ post.title }}</a>
<a class="team-pos">{{ post.date | date: "%-d %B %Y" }}</a>
<div class="team-text" style="height: 80px">{{ post.description }}</div>
</div>
</div>
{% endfor %}