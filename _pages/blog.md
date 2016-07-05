---
permalink: /blog/
layout: archive
title: "Improve your Eye Wellbeing"
excerpt: "Friederike Wild your coach for eye wellbeing for healthy and vital vision."
author_profile: true
sitemap: true
read_time: false
comments: false
share: true
related: false

header:
  overlay_color: "#8492cd"
  overlay_image: home-page-feature.jpg

---

{% include base_path %}

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts }}</h3>

<div class="grid__wrapper">
  {% for post in site.posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

{% include archive-single.html %}
