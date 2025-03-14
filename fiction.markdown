---
layout: default
title: Fiction
permalink: /fiction/
---
<head>
  <link rel="stylesheet" href="{{ "/assets/css/style.css" | relative_url }}">
</head>

<h1 class="page-title">Fiction</h1>

<div class="fiction-grid">
  {% for story in site.fiction %}
  <div class="fiction-card">
    <a href="{{ story.url }}">
      <h2>{{ story.title }}</h2>
    </a>
    <p class="fiction-date">{{ story.date | date: "%B %d, %Y" }}</p>
    <p class="fiction-excerpt">{{ story.excerpt | strip_html }}</p>
  </div>
  {% else %}
    <p>No fiction pieces available yet.</p>
  {% endfor %}
</div>
