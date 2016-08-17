---
title: "Writing About Dark Souls"
layout: archive
author_profile: true
excerpt: "Writing about Dark Souls."
permalink: /darksouls-alt/
---

{% include base_path %}
{% assign darksouls = site.data.darksouls[include.darksouls] %}

{% for article in site.data.darksouls %}
  <h2>{{ article.title }}</h2>
  {% for subcategory in entry.subcategories %}
    <h3>{{ subcategory.title }}</h3>
    
  {% endfor %}
{% endfor %}