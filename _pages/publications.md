---
layout: archive
title: "First-author publications"
permalink: /publications/
author_profile: true
---
<div style="font-family: Calibri, serif; font-size: 0.9rem;">
{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}
</div>

{% include base_path %}

<div style="font-family: Calibri, serif; font-size: 0.9rem;">
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
</div>
