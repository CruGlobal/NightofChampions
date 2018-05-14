---
title: Silent Auction
date: 2017-11-13 14:52:00 Z
position: 6
description: Auction will be held prior to the start of the event.
---

### Sports Memorabilia Items
{% assign sorted = site.silent-auction | sort: 'title' %}
{% for post in sorted %}
{% if post.type == "sports" %}
<div class="col-xs-6 col-md-6">
    <div style="padding-bottom: 30px;">
        <img src="{{ post.image }}" alt="">
        <h4>{{ post.title }}</h4>
    </div>
</div>
{% endif %}
{% endfor %}