---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

A selection of my research articles, conference papers, and other academic works.

{% assign publications = site.publications | sort: "date" | reverse %}

{% for post in publications %}
  {% if post.title and post.venue and post.date %}
    <div class="list__item">

      <h2 class="archive__item-title">
        {% if post.paperurl %}
          <a href="{{ post.paperurl }}" target="_blank" rel="noopener">
            {{ post.title }}
          </a>
        {% else %}
          {{ post.title }}
        {% endif %}
      </h2>

      <p>
        Published in <em>{{ post.venue }}</em>, {{ post.date | date: "%Y" }}
      </p>

    </div>
  {% endif %}
{% endfor %}
