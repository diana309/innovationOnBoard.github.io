---
layout: sponsor_page
title: Sponsors
description: Sponsors and Community Supporters
image: /assets/images/pic05.jpg
redirect_from:
#   - /sponsors
#   - /sponsors.html
tag: ubc
weight: 2
---

<!-- <h1 style="color: #2a2f4a !important;">Sponsors</h1>  -->

<h1 style="color: #2a2f4a !important;">Sponsors & Partners 2024-2025</h1>

<div class="row">
{% assign sponsors = site.sponsors | where: 'campus', 'ubc' | sort: 'weight' %}
{% for sponsor in sponsors %}
	{% if sponsor.status == 'present' %}
		<div class="2u" style="text-align:center;">
			<span class="image fit">
            <a href="{{ sponsor.link }}">
				<img src="{{ sponsor.img | prepend: site.baseurl | prepend: site.url }}" class="img">
            </a>
			</span>
		</div>
	{% endif %}
{% endfor %}
</div>

<h1 style="color: #2a2f4a !important; padding-top: 2.5rem;">Past Sponsors & Partners</h1>
<div class="row">
{% assign sponsors = site.sponsors | sort: 'weight' %}
{% for sponsor in sponsors %}
{% if sponsor.status == 'past' %}
		<div class="2u" style="text-align:center;">
			<span class="image fit">
				<img src="{{ sponsor.img | prepend: site.baseurl | prepend: site.url }}" class="img-sponsor">
			</span>
		</div>
		{% endif %}
{% endfor %}

<hr>
