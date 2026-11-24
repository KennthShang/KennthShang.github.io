---
layout: default
title: Publications
description: Publications by Jiayu Shang in computational biology, bioinformatics, and machine learning.
nav: publications
permalink: /publication.html
---
<div class="container archive">
  <header class="page-heading">
    <h1>Publications</h1>
    <p>For a full publication list, see <a href="{{ site.scholar }}">Google Scholar</a> or my <a href="{{ site.cv | relative_url }}">CV</a>.</p>
  </header>
  {% assign years = site.data.publications | group_by: 'year' %}
  {% for year in years %}
  <section class="year-group" aria-labelledby="papers-{{ year.name }}">
    <h2 id="papers-{{ year.name }}">{{ year.name }}</h2>
    <ul class="record-list">
      {% for paper in year.items %}
        {% include publication.html paper=paper %}
      {% endfor %}
    </ul>
  </section>
  {% endfor %}
</div>
