---
layout: default
---

<article class="fiction-story">
  <h1 class="story-title">{{ page.title }}</h1>
  <p class="story-date">{{ page.date | date: "%B %d, %Y" }}</p>
  
  <div class="story-content">
  

     {% if page.excerpt %}
      <p class="story-excerpt"><em>{{ page.excerpt }}</em></p>
    {% endif %}

    {% if page.image %}
      <img src="{{ page.image }}" alt="{{ page.title }}" class="story-image">
    {% endif %}
    
    {{ content }}
  </div>
</article>
