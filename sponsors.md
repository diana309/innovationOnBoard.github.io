---
layout: sponsor_page
title: Sponsors of the 2017/2018 cohort
description: Sponsors and Community Supporters
image: assets/images/pic05.jpg
---

<div class="row">
{% for sponsor in site.sponsors %}
	{% if sponsor.status == '2023-2024' %}
		<div class="4u 12u$(small)" style="text-align:center;">
			<span class="image fit">
				<img src="{{ sponsor.img | prepend: site.baseurl | prepend: site.url }}" class="img-sponsor">
			</span>
		</div>
	{% endif %}
{% endfor %}
</div>

<hr>

<div class="row">
{% for sponsor in site.sponsors %}
	{% if sponsor.status == 'gold' %}
		<div class="4u 12u$(small)" style="text-align:center;">
			<span class="image fit">
				<img src="{{ sponsor.img | prepend: site.baseurl | prepend: site.url }}" class="img-sponsor">
			</span>
		</div>
	{% endif %}
{% endfor %}
</div>

<hr>

<div class="row">
{% for sponsor in site.sponsors %}
	{% if sponsor.status == 'silver' %}
		<div class="4u 12u$(small)" style="text-align:center;">
			<span class="image fit">
				<img src="{{ sponsor.img | prepend: site.baseurl | prepend: site.url }}" class="img-sponsor">
			</span>
		</div>
	{% endif %}
{% endfor %}
</div>

<hr>

<div class="row">
{% for sponsor in site.sponsors %}
	{% if sponsor.status == 'partner' %}
		<div class="4u 12u$(small)" style="text-align:center;">
			<span class="image fit">
				<img src="{{ sponsor.img | prepend: site.baseurl | prepend: site.url }}" class="img-sponsor">
			</span>
		</div>
	{% endif %}
{% endfor %}
</div>
