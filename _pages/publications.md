---
layout: archive
title: "First-authored publications"
permalink: /publications/
author_profile: true
---
{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<div style="font-size: 0.9rem;">
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
</div>

