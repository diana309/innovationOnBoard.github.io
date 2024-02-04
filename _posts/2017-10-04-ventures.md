---
layout: venture
title: Ventures in 2017/2018 & 2023/2024 
description: Ventures in 2017/2018 & 2023/2024
image: assets/images/pic13.jpg
redirect_from: "/ventures/"
---
{% assign members = site.members | sort: 'weight' %}


<!-- ## Ventures of the 2017/2018 cohort -->
<div class="row">
{% assign members = site.members | where:"status", "ventures" | sort: 'weight' %}
{% for member in members %}
	<div class="16u 12u$(small)" style="text-align:center;"><div class="box">
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
	</div></div> {% unless forloop.last %}{% cycle '', '', '</div><div class="row">' %}{% endunless %}
{% endfor %}
</div>
