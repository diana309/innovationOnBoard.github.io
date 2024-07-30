---
layout: post
title: Board Members
description: Innovation OnBoard Organizers
image: /assets/images/pic01.jpg
redirect_from: "/board"
explanation: Meet our board members who help us execute our mission with passion and dedication, providing invaluable guidance and expertise. Their collective experience and strategic vision ensure our continued success and growth.
tag: home
weight: 4
---

{% assign members = site.members | sort: 'weight' %}

<!-- ## Board of Advisors -->
<div class="row">
{% assign members = site.members | where:"status", "board" | sort: 'weight' %}
{% for member in members %}
	<div class="4u 12u$(small)" style="text-align:center;"><div class="box">
	<img src="{{ member.img | prepend: site.baseurl | prepend: site.url }}" class="img-team" style="width: 200px; height: 200px;">
	<h4>{{ member.name }}
	<p><i>{{ member.title }} | </i>
	{% if site.linkedin_url %}
	<a href="{{ member.linkedin }}" class="icon fa-linkedin" target="_blank"><span class="label">LinkedIn</span></a>
	{% endif %}
	</p>
	</h4>
	<hr>
	<p>{{ member.biography }}</p>
	</div></div> {% unless forloop.last %}{% cycle '', '', '</div><div class="row">' %}{% endunless %}
{% endfor %}

</div>
