---
layout: default
---

<div class="small-container text-center">
  {% for post in site.categories["公告"] %}
    <a href="{{ site.baseurl }}{{ post.url }}" class="article-link">
      <article class="article-excerpt">
        <img src="{{ post.image }}" alt="{{post.title}}">      
        <div>
          <h1>{{ post.title }}</h1>
          <time>{{ post.date | date: "%B %e, %Y" }}</time>
          <p>
            {{ post.excerpt | strip_html }}
          </p>
        </div>
      </article>
    </a>
  {% endfor %}
</div>