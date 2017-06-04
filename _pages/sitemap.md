---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: false

---

{% include base_path %}

A list of all the posts and pages found on the site. There is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well for you robots out there.

<h2>Pages</h2>
{% for post in site.pages %}
  {% if post.sitemap %}
	{% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Posts</h2>
{% for post in site.posts %}
  {% if post.sitemap %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
{% unless collection.output == false or collection.label == "posts" %}
  {% capture label %}{{ collection.label }}{% endcapture %}
  {% if label != written_label %}
  <h2>{{ label }}</h2>
  {% capture written_label %}{{ label }}{% endcapture %}
  {% endif %}
{% endunless %}
{% for post in collection.docs %}
  {% unless collection.output == false or collection.label == "posts" %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}
{% endfor %}