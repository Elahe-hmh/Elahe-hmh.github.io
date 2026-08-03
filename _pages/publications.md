---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}


A selection of my research articles, conference papers, and other academic works.


{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
