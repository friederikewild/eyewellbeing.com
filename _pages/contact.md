---
permalink: /contact/
title: "Let’s connect!"
layout: single
excerpt: "Looking forward to connect with you. Find me on Facebook, Instagram and Twitter. Or reach out to me via email."
modified: 2016-07-05T13:20:00-1:00

---

{% include base_path %}


{% if page.author %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}

[comment]: <> (TODO: Add a nice photo header?)

<div class="author__urls-wrapper">
<ul class="author__urls social-icons">

{% if author.facebook %}
        <li><a href="https://www.facebook.com/{{ author.facebook }}/?ref=webf"><i class="fa fa-facebook" aria-hidden="true"></i> Facebook</a></li>
{% endif %}
      
{% if author.google_plus %}
        <li><a href="https://plus.google.com/+{{ author.google_plus }}"><i class="fa fa-circle fa-google-plus" aria-hidden="true"></i> Google+</a></li>
{% endif %}

{% if author.instagram %}
        <li><a href="https://instagram.com/{{ author.instagram }}"><i class="fa fa-circle fa-instagram" aria-hidden="true"></i> Instagram</a></li>
{% endif %}

{% if author.twitter %}
        <li><a href="https://twitter.com/{{ author.twitter }}"><i class="fa fa-twitter" aria-hidden="true"></i> Twitter</a></li>
      {% endif %}
      
{% if author.linkedin %}
        <li><a href="https://www.linkedin.com/in/{{ author.linkedin }}"><i class="fa fa-linkedin" aria-hidden="true"></i> LinkedIn</a></li>
{% endif %}

{% if author.xing %}
        <li><a href="https://www.xing.com/profile/{{ author.xing }}"><i class="fa fa-circle fa-xing" aria-hidden="true"></i> XING</a></li>
{% endif %}

      
</ul>
</div>

[comment]: <> (Add email form...)
[comment]: <> (Might want different formatting<span class="fa-stack fa-lg"><i class="fa fa-circle fa-stack-2x"></i><i class="fa fa-instagram fa-stack-1x fa-inverse"></i></span> )
