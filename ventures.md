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
@media screen and (min-width: 800px) {
    .flex-container {
        display: flex;
        flex-wrap: wrap;
    }
    .flex-item {
                flex: 1 0 calc(50% - 10px);
                box-sizing: border-box;
                padding: 10px;
    }

    .kpi-container {
        display: flex;
        flex-wrap: wrap;
        padding: 10px;
        padding-bottom: 50px;
        gap: 40px;
    }
    .kpi-box {
        border: 1px solid #ccc; 
        display: flex;
        align-items: center;
        padding-left: 20px;
        padding-right: 20px;
        padding-top: 10px;
        padding-bottom: 10px;
    }
}
</style>

<h1>Ventures 2023-2024</h1>
<div class="kpi-container">
    <div class="kpi-box">
       <b>Teams Registered: 52</b> 
    </div>
    <div class="kpi-box">
       <b>Total Attended: 1000+</b> 
    </div>
    <div class="kpi-box">
        <b>Total Faculties: 20</b>
    </div>
</div>
<div class="flex-container">
{% assign members = site.members | where:"status", "ventures" | where:"title", "2023 cohort" | sort: 'weight' %}
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

<h1>Ventures 2017-2018</h1>
<div class="flex-container">
{% assign members = site.members | where:"status", "ventures" | where:"title", "2017 cohort" | sort: 'weight' %}
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
