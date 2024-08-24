---
layout: venture
title: Ventures
description: Ventures in 2017/2018 & 2023/2024
image: /assets/images/pic13.jpg
redirect_from: "/ventures/"
tag: home
weight: 3
---

{% assign members = site.members | sort: 'weight' %}

<style>
.flex-container {
    display: flex;
    flex-wrap: wrap;
}
.flex-item {
            flex: 1 1 calc(50% - 10px); /* Two items per row, accounting for gap */
            box-sizing: border-box; /* Include padding and border in the width */
            padding: 10px;
        }
</style>

<div class="flex-container">
{% assign members = site.members | where:"status", "ventures" | sort: 'weight' %}
{% for member in members %}
    <div class="flex-item" style="text-align:center;">
        <div class="box">
            <img src="{{ member.img | prepend: site.baseurl | prepend: site.url }}" class="img-sponsor" style="width: 600px; height: 450px;">
            <h4>{{ member.name }}
            <p><i>{{ member.title }} </i>
        <!-- {% if site.linkedin_url %}
            <a href="{{ member.linkedin }}" class="icon fa-linkedin" target="_blank"><span class="label">LinkedIn</span></a>
            {% endif %} -->
            </p>
            </h4>
            <hr>
            <p>{{ member.biography }}</p>
        </div>
    </div>

{% endfor %}

</div>
