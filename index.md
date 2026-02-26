---
layout: page
title: ""
subtitle: ""
---

<div class="home-hero">
  <div class="home-hero__title">Aaron Graifman</div>
  <div class="home-hero__subtitle">Data Analyst · Program Evaluation · Decision Systems</div>

  <div class="home-hero__blurb">
    I build operational analytics systems for public-sector decision making:
    administrative data pipelines, evaluation frameworks, forecasting models,
    and reproducible reporting workflows in R.
  </div>

  <div class="home-cta">
    <a class="btn btn-primary btn-lg" href="/cv/">View CV</a>
    <a class="btn btn-outline-primary btn-lg" href="/academic-projects/">Academic Projects</a>
    <a class="btn btn-outline-primary btn-lg" href="/tools/">Tools</a>
  </div>
</div>

<div class="home-section">
  <h2>Featured Academic Work</h2>

  {% assign featured = site.academic_projects | where: "featured", true | sort: "order" %}

  <div class="card-grid">
    {% for p in featured %}
      <div class="card">
        <div class="card__title">
          <a href="{{ p.url }}">{{ p.short_title | default: p.title }}</a>
        </div>

        {% if p.meta %}
          <div class="card__meta">{{ p.meta }}</div>
        {% endif %}

        <div class="card__text">
          {% if p.summary %}
            {{ p.summary }}
          {% else %}
            {{ p.excerpt | strip_html | truncate: 170 }}
          {% endif %}
        </div>

        <div class="card__links">
          <a href="{{ p.url }}">Read more →</a>
        </div>
      </div>
    {% endfor %}
  </div>
</div>

<div class="home-section">
  <h2>Focus</h2>
  <ul class="home-bullets">
    <li>Evaluation design grounded in administrative data systems</li>
    <li>Equity-aware measurement and implementation analysis</li>
    <li>R (tidyverse), RMarkdown, Git/GitHub</li>
    <li>Forecasting, segmentation, and decision-ready reporting</li>
  </ul>
</div>
