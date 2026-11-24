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

  <section class="section" id="about" aria-labelledby="about-title">
    <h2 id="about-title">About</h2>
    <div class="prose">
      <p>I am a postdoctoral fellow in the Department of Information Engineering at The Chinese University of Hong Kong. In January 2027, I will join the Artificial Intelligence Thrust at the Information Hub of The Hong Kong University of Science and Technology (Guangzhou) as an assistant professor. I received my PhD in Electrical Engineering from City University of Hong Kong, where I was advised by <a href="https://yannisun.github.io/">Prof. Yanni Sun</a>, and completed my undergraduate studies at Sun Yat-sen University.</p>
      <p>I develop machine learning methods and bioinformatics tools to study microbial communities and interpret biological sequences. I use large-scale sequencing data to characterize microbial and viral diversity, infer protein function, and investigate links between the human gut microbiome and disease.</p>
    </div>
  </section>

  <section class="section" id="research" aria-labelledby="research-title">
    <div class="section-heading">
      <h2 id="research-title">Research interests</h2>
      <a class="text-link" href="{{ '/research.html' | relative_url }}">Explore research projects</a>
    </div>
    <div class="research-grid">
      <article>
        <img src="{{ '/assets/research/microbial-genomics.webp' | relative_url }}" alt="" width="768" height="512" loading="lazy" decoding="async">
        <div class="research-card-copy">
          <h3>Microbial genomics</h3>
          <ul>
            <li>Microbial community profiling in host-associated and environmental metagenomes</li>
            <li>Gene-centric analysis of microbial functions</li>
            <li>Viral diversity, classification, and host associations</li>
          </ul>
        </div>
      </article>
      <article>
        <img src="{{ '/assets/research/sequence-learning.webp' | relative_url }}" alt="A researcher views a diagram of a neural network using an amino acid sequence to predict a protein annotation." width="768" height="512" loading="lazy" decoding="async">
        <div class="research-card-copy">
          <h3>Machine learning for sequences</h3>
          <ul>
            <li>Deep learning for biological sequence analysis</li>
            <li>Protein function prediction and genome annotation</li>
            <li>Algorithms and tools for large-scale genomic data</li>
          </ul>
        </div>
      </article>
      <article>
        <img src="{{ '/assets/research/precision-health.webp' | relative_url }}" alt="Concept drawing of a phage medicine vial and a magnified gut scene showing a phage lysing a target bacterium." width="768" height="512" loading="lazy" decoding="async">
        <div class="research-card-copy">
          <h3>AI for precision health</h3>
          <ul>
            <li>Links between the gut microbiome and disease</li>
            <li>AI-guided phage design to target disease-associated bacteria</li>
            <li>Assessing effects on the wider gut microbiome</li>
          </ul>
        </div>
      </article>
    </div>
  </section>

  <section class="section" id="news" aria-labelledby="news-title">
    <div class="section-heading">
      <h2 id="news-title">Recent News</h2>
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
</div>
