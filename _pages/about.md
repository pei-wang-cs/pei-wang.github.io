---
permalink: /
layout: home
title: "About Me"
description: "Pei Wang is a Ph.D. student at Tsinghua University researching formal verification and concurrent programs."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<section id="about" class="home-section" aria-labelledby="about-heading" markdown="1">

<h1 id="about-heading" class="section-title"><span class="fa-solid fa-user-graduate" aria-hidden="true"></span> About Me</h1>

Hi! I am **Pei Wang**, a Ph.D. student at the School of Software, Tsinghua University, and a member of the [Formal Verification Lab](https://thufv.github.io/). I joined the Ph.D. program in 2023.

My research focuses on **formal methods and concurrent program verification**, especially precise and efficient analysis of concurrency bugs such as **deadlocks** and **data races**.

You can reach me at [{{ site.author.email }}](mailto:{{ site.author.email }}).

</section>

<section id="news" class="home-section" aria-labelledby="news-heading">
  <h2 id="news-heading" class="section-title"><span class="fa-solid fa-bullhorn" aria-hidden="true"></span> News</h2>
  <ul class="news-list">
    <li>
      <time datetime="2026-10">10/2026</time>
      <div>Our paper “<a href="{{ '/publication/precise-efficient-static-data-race-detection/' | relative_url }}">Precise and Efficient Static Data Race Detection</a>” was published in the <strong>ASE 2026</strong> proceedings. <a href="https://doi.org/10.1145/3832783.3837438">[Paper]</a> <a href="https://doi.org/10.5281/zenodo.21775785">[Artifact]</a></div>
    </li>
    <li>
      <time datetime="2026-07">07/2026</time>
      <div>Our paper “<a href="{{ '/publication/deadlock-verification-ordering-constrained-mutex-modeling/' | relative_url }}">Deadlock Verification via Ordering-Constrained Mutex Modeling</a>” was published at <strong>CAV 2026</strong>. <a href="https://doi.org/10.1007/978-3-032-32519-8_3">[Paper]</a> <a href="https://doi.org/10.5281/zenodo.19696864">[Artifact]</a></div>
    </li>
  </ul>
</section>

<section id="publications" class="home-section" aria-labelledby="publications-heading">
  <h2 id="publications-heading" class="section-title"><span class="fa-solid fa-book-open" aria-hidden="true"></span> Publications</h2>
  <p class="section-note">See also <a href="{{ site.author.googlescholar | escape }}">Google Scholar</a> for my research.</p>
  <div class="publications">
    {% assign publications_by_year = site.publications | sort: 'date' | reverse | group_by_exp: 'post', "post.date | date: '%Y'" %}
    {% for year in publications_by_year %}
      <div class="publications__year-group">
        <h3 class="publications__year">{{ year.name }}</h3>
        {% for post in year.items %}
          {% include publication-list-item.html compact=true heading_level=4 %}
        {% endfor %}
      </div>
    {% endfor %}
  </div>
  <p class="all-publications"><a href="{{ '/publications/' | relative_url }}">All publications <span aria-hidden="true">→</span></a></p>
</section>
