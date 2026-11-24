---
layout: default
title: News
description: Research updates and publication announcements from Jiayu Shang.
nav: news
permalink: /News.html
---
<div class="container archive">
  <header class="page-heading">
    <h1>News</h1>
    <p>Research updates, publications, and software releases.</p>
  </header>
  <div class="record-list">
    {% for update in site.data.news %}
    <article class="record news-entry" id="{{ update.id }}">
      <time class="record-meta" datetime="{{ update.date }}">{{ update.date | date: '%b %d, %Y' }}</time>
      <div>
        <h2>{{ update.title | escape }}</h2>
        <p class="news-summary">{{ update.summary | escape }}</p>
        <div class="news-links">
          {% for link in update.links %}
          <a class="text-link" href="{{ link.url | escape }}">{{ link.label | escape }}</a>
          {% endfor %}
        </div>
      </div>
    </article>
    {% endfor %}
  </div>
</div>
