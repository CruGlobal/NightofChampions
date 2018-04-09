---
title: Sponsors
date: 2017-11-13 14:51:00 Z
position: 3
---


<div class="row text-center">
    <h3>Presenting Sponsors</h3>
    {% for post in site.sponsors %}
    {% if post.level == "Presenting" %}
    <div class="no-padding col-xs-6 col-md-6" style="display: inline-block; float: none;">
        <div style="padding-bottom: 30px;">
            <img src="{{ post.image }}" alt="">
            <p style="padding-top: 15px;">{{ post. quote }}</p>
        </div>
    </div>
    {% endif %}
    {% endfor %}
</div>
<div class="row text-center">
    <h3>Team Sponsors</h3>
    {% assign sorted = site.sponsors | sort: 'title' %}
    {% for post in sorted %}
    {% if post.level == "Team" %}
    <div class="no-padding col-xs-6 col-md-3" style="display: inline-block; float: none;">
        <div style="padding-bottom: 30px;">
            <img src="{{ post.image }}" alt="">
        </div>
    </div>
    {% endif %}
    {% endfor %}
</div>