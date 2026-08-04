---
layout: archive
title: "Publications and Awards"
permalink: /publications/
author_profile: true
---

<style>
.award-group {
  margin-top: 1.5rem;
}

.award-item {
  margin: 0 0 1.6rem 0;
  padding: 0.2rem 0 0.2rem 1rem;
  border-left: 3px solid #2c7f95;
}

.award-header {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  gap: 1rem;
}

.award-title {
  font-size: 1.05rem;
  font-weight: 700;
}

.award-year {
  white-space: nowrap;
  color: #666;
  font-weight: 600;
}

.award-institution {
  margin-top: 0.2rem;
  color: #666;
  font-size: 0.95rem;
}

.award-description {
  margin-top: 0.45rem;
  line-height: 1.55;
}

@media (max-width: 600px) {
  .award-header {
    display: block;
  }

  .award-year {
    display: block;
    margin-top: 0.2rem;
  }
}
</style>

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

## Awards, Fellowships, and Scholarships

<div class="award-group">

  <div class="award-item">
    <div class="award-header">
      <span class="award-title">
        Anona Thorne and Takao Tanabe Graduate Entrance Scholarship
      </span>
      <span class="award-year">October 2024</span>
    </div>

    <div class="award-institution">
      University of British Columbia
    </div>

    <div class="award-description">
      Selected as a recipient of the Anona Thorne and Takao Tanabe
      Graduate Entrance Scholarship.
    </div>
  </div>

  <div class="award-item">
    <div class="award-header">
      <span class="award-title">
        IAEA Marie Skłodowska-Curie Fellowship Programme
      </span>
      <span class="award-year">2022–2025</span>
    </div>

    <div class="award-institution">
      International Atomic Energy Agency
    </div>

    <div class="award-description">
      Selected for the IAEA Marie Skłodowska-Curie Fellowship Programme.
    </div>
  </div>


  <div class="award-item">
    <div class="award-header">
      <span class="award-title">
        First Place in the NeuroTract Competition
      </span>
      <span class="award-year">2019</span>
    </div>

    <div class="award-institution">
      Tehran University of Medical Sciences
    </div>

    <div class="award-description">
      Received first place for the research project presented during the
      NeuroTract program.
    </div>
  </div>

  <div class="award-item">
    <div class="award-header">
      <span class="award-title">
        Winner of the Second National Neuroscience Competition
      </span>
      <span class="award-year">2018</span>
    </div>

    <div class="award-institution">
      IPM Institute for Research
    </div>

    <div class="award-description">
      Recognized for the project proposal
      <em>Olfactory Modeling with Directed Graphs</em>.
    </div>
  </div>

</div>
