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
        <div class="news-body">{{ update.body | markdownify }}</div>
      </div>
    </article>
    {% endfor %}
  </div>
</div>
