---
layout: default
title: All Articles
permalink: /articles/
---

# Articles

<section class="articles">
  {% for post in site.posts %}
    <div class="article">
      <a href="{{ post.url }}">
				{{ post.title }}
			</a>
    </div>
  {% endfor %}
</section>