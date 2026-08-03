---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## Publications

My research articles, conference papers, and other academic works.

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

---

## Awards

### Anona Thorne and Takao Tanabe Graduate Entrance Scholarship
**University of British Columbia — October 2024**

Selected as a recipient of the Anona Thorne and Takao Tanabe Graduate Scholarship.

### IAEA Marie Skłodowska-Curie Fellowship Programme
**International Atomic Energy Agency — 2022–2025**

Selected for the IAEA Marie Skłodowska-Curie Fellowship Programme.

### First Place in Neurotract International Summer School
**Tehran University of Medical Sciences — 2019**

Participated in the Neurotract International Summer School in Tehran and won as the best project in their competition.


### National Neuroscience Competition
**IPM Institute for Research — 2018**

Awarded for the project proposal *Olfactory Modeling with Directed Graphs*.
