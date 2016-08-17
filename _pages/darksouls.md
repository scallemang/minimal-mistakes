---
title: "Writing About Dark Souls"
layout: archive
author_profile: true
excerpt: "Writing about Dark Souls."
permalink: /darksouls/
---

{% include base_path %}

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts }}</h3>

{% for post in site.data.darksouls.articles %}
  {% include archive-single.html %}
  {% if post.tags[0] %}
    {% include tag-list-archive.html %}
  {% endif %}

  {% if site.category_archive.type and page.categories[0] %}
    {% include category-list.html %}
  {% endif %}
{% endfor %}