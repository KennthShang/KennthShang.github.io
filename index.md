---
layout: default
title: Jiayu Shang
nav: home
permalink: /
---
<div class="container">
  <section class="hero" aria-labelledby="profile-name">
    <div class="hero-copy">
      <p class="eyebrow">Computational biology &amp; bioinformatics</p>
      <h1 id="profile-name">Jiayu Shang</h1>
      <div class="hero-affiliation">
        <p class="hero-role">Postdoctoral Fellow</p>
        <p>Department of Information Engineering<br>The Chinese University of Hong Kong</p>
      </div>
      <p class="hero-appointment"><strong>Starting January 2027</strong><br>Assistant Professor, AI Thrust, HKUST (Guangzhou)</p>
      <ul class="profile-links" aria-label="Contact and academic profiles">
        <li><a class="button button-primary" href="mailto:{{ site.email }}">Email</a></li>
        <li><a class="button button-outline" href="{{ site.scholar }}">Google Scholar</a></li>
        <li><a class="button button-outline" href="{{ site.github_profile }}">GitHub</a></li>
      </ul>
    </div>
    <div class="portrait-frame">
      <img class="portrait" src="{{ '/assets/portrait.jpg' | relative_url }}" alt="Portrait of Jiayu Shang" width="900" height="900" fetchpriority="high">
    </div>
  </section>

  <section class="section about-grid" id="about" aria-labelledby="about-title">
    <div>
      <h2 id="about-title">About</h2>
      <p>I develop machine learning methods and bioinformatics tools to make sense of large-scale biological sequence data. My work spans microbial metagenomics, protein annotation, and high-throughput sequencing analysis.</p>
      <p>I earned my PhD in Electrical Engineering at City University of Hong Kong under the supervision of <a href="https://scholar.google.com/citations?user=1wloHDIAAAAJ">Yanni Sun</a> and completed my undergraduate studies at Sun Yat-sen University.</p>
    </div>
    <div class="academic-background">
      <h3>Academic background</h3>
      <ul class="background-list">
        <li><strong>Postdoctoral Fellow</strong><span>The Chinese University of Hong Kong</span></li>
        <li><strong>PhD, Electrical Engineering</strong><span>City University of Hong Kong</span></li>
        <li><strong>BEng</strong><span>Sun Yat-sen University</span></li>
      </ul>
    </div>
  </section>

  <section class="section" id="research" aria-labelledby="research-title">
    <h2 id="research-title">Research interests</h2>
    <div class="research-grid">
      <article>
        <h3>Microbial genomics</h3>
        <p>Analyzing high-throughput sequencing data to characterize microbial communities and viral diversity.</p>
      </article>
      <article>
        <h3>Machine learning for sequences</h3>
        <p>Learning efficient representations of biological sequences for protein and genome annotation.</p>
      </article>
      <article>
        <h3>AI for public and precision health</h3>
        <p>Studying environmental microbiomes and exploring links between the human microbiome and disease.</p>
      </article>
    </div>
  </section>

  <section class="section" id="publications" aria-labelledby="publications-title">
    <div class="section-heading">
      <h2 id="publications-title">Selected publications</h2>
      <a class="text-link" href="{{ '/publication.html' | relative_url }}">Publication archive</a>
    </div>
    <ul class="record-list">
      {% assign selected_papers = site.data.publications | where: 'selected', true %}
      {% for paper in selected_papers %}
        {% include publication.html paper=paper show_year=true %}
      {% endfor %}
    </ul>
  </section>

  <section class="section" id="news" aria-labelledby="news-title">
    <div class="section-heading">
      <h2 id="news-title">News</h2>
      <a class="text-link" href="{{ '/News.html' | relative_url }}">News archive</a>
    </div>
    <ul class="record-list">
      {% for update in site.data.news limit:3 %}
      <li class="record">
        <time class="record-meta" datetime="{{ update.date }}">{{ update.date | date: '%b %d, %Y' }}</time>
        <div>
          <h3><a class="record-title" href="{{ '/News.html' | relative_url }}#{{ update.id }}">{{ update.title | escape }}</a></h3>
          <p>{{ update.summary | escape }}</p>
        </div>
      </li>
      {% endfor %}
    </ul>
  </section>
</div>
