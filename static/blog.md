---
layout: blog
title: blog
permalink: /blog
---

# tags

{% for tag in site.tags %}

  {% assign tag_slug = tag | first %}
  {% assign no_of_posts = tag | last | size %}

  <a href="{{ 'tag/' | relative_url }}{{ tag_slug }}" title="See all posts by {{ tag_slug }} tag">#{{ tag_slug
            }}</a>
{% endfor %}

# articles
