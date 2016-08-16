---
title: "Scroll Locations, or The Dork&rsquo;s Archives"
layout: archive
author_profile: true
excerpt: "Writing about Dark Souls."
permalink: /darksouls/
---

{% include base_path %}

<p>Writing About From Software&rsquo;s Souls Series (Demon Souls, Dark Souls I, II and III, Bloodborne)</p>

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts }}</h3>

{% for post in site.darksouls %}
  {% include archive-single.html %}
  {% if post.tags[0] %}
	  {% include tag-list.html %}
	{% endif %}

	{% if site.category_archive.type and page.categories[0] %}
	  {% include category-list.html %}
	{% endif %}
{% endfor %}

{% include paginator.html %}