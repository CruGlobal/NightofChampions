---
title: Sponsors
date: 2017-11-13 14:51:00 Z
position: 3
---

### Presenting Sponsors
<div class="row text-center">
    {% for post in site.sponsors %}
    {% if post.level == "Presenting" %}
    <div class="no-padding col-xs-6 col-md-6" style="display: inline-block; float: none;">
        <div class="sponsor-entry">
            <img src="{{ post.image }}" alt="">
            <br />
            {{ post. quote }}
        </div>
    </div>
    {% endif %}
    {% endfor %}
</div>
### Team Sponsors
<div class="row text-center">
    {% assign sorted = site.sponsors | sort: 'title' %}
    {% for post in sorted %}
    {% if post.level == "Team" %}
    <div class="no-padding col-xs-6 col-md-3" style="display: inline-block; float: none;">
        <div class="sponsor-entry">
            <img src="{{ post.image }}" alt="">
        </div>
    </div>
    {% endif %}
    {% endfor %}
</div>