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
  <div class="list__item">
    <h2 class="archive__item-title">
      {{ post.title }}
    </h2>

    <p>
      Published in <em>{{ post.venue }}</em>, {{ post.date | date: "%Y" }}
    </p>

    {% if post.paperurl %}
      <p>
        <a href="{{ post.paperurl }}" target="_blank" rel="noopener">
          View paper
        </a>
      </p>
    {% endif %}
  </div>
{% endfor %}
