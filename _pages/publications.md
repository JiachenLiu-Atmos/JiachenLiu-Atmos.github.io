---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<section class="pub-hero">
  <p class="eyebrow">First-authored papers</p>
  <p>Climate dynamics, clouds, hothouse hydrology, and 3D transport-induced chemistry on exoplanets.</p>
  {% if site.author.googlescholar %}
    <a class="pub-button" href="{{ site.author.googlescholar }}">Google Scholar</a>
  {% endif %}
</section>

{% include base_path %}

<section class="publication-list" aria-label="Publication list">
  {% for post in site.publications reversed %}
    <article class="publication-card">
      <div class="publication-meta">
        {% if post.date %}<span>{{ post.date | date: "%Y" }}</span>{% endif %}
        {% if post.venue %}<span>{{ post.venue }}</span>{% endif %}
      </div>
      <h2><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></h2>
      {% if post.excerpt and post.excerpt != "" %}
        <p class="publication-summary">{{ post.excerpt }}</p>
      {% endif %}
      <div class="publication-actions">
        <a href="{{ base_path }}{{ post.url }}">Details</a>
        {% if post.paperurl %}<a href="{{ post.paperurl }}">PDF</a>{% endif %}
      </div>
    </article>
  {% endfor %}
</section>
