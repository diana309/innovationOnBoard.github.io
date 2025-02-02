---
layout: university_page
title: University of British Columbia
short-title: UBC
landing-title: " "
description: IOB AT UNIVERSITY OF BRITISH COLUMBIA
image: assets/images/pic13.jpg
author: null
tag: home
weight: 1
---

<!-- Main -->

{% include header.html %}

  <section id="banner" class="banner-sponsor">
    <div class="inner">
      <header class="major">
        <h1>{{ page.title }}</h1>
      </header>
      <p>
       Innovation OnBoard is a student-led entrepreneurship program featuring bi-weekly seminars and workshops, culminating in a premier venture competition where teams compete for cash prizes. We foster innovation by providing a forum to build cohesive, multidisciplinary teams, simplify the entrepreneurial experience, and launch new ventures.
      </p>
    </div>
  </section>
<div id="main" class="alt">
    <section id="one" class="alt">
      <div class="inner">
        <header>
          <div class="row">
            <div class="6u 12u$(small)">
              <div class="box">
                <h1>Workshops Sign Up</h1>
                <p>
                  Unlock the path to entrepreneurship, connect with fellow startup enthusiasts, and gain valuable
                  insights from experienced entrepreneurs and industry experts. Sign up to receive event reminders.
                </p>
                <ul class="actions fit">
                  <li>
                    <a href="{{ '/participant-signup.html' | prepend: site.baseurl | prepend: site.url }}"
                      target="_blank" class="button fit">Sign Up</a>
                  </li>
                </ul>
              </div>
            </div>
            <div class="6u 12u$(small)">
              <div class="box">
                <h1>Join the IOB Team</h1>
                <p> Looking to get involved in an exciting project? Apply now, and we’ll reach out to you via email. Joining IOB is a fantastic opportunity to build valuable experience. 
                  <br>
                </p>
                <br>
                <ul class="actions fit">
                  <li>
              <a href="{{ '/job-posting' | prepend: site.baseurl | prepend: site.url }}" class="button fit"
                  style="color: white; background-color:#002047">Apply Here</a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </header>
      </div>
    </section>
</div>

{% include tiles.html page="ubc" %}
