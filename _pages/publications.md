---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<!-- New style rendering if publication categories are defined -->

<h2>Books and Monographs</h2><hr />
{% for post in site.publications reversed %}
  {% if post.category == 'books' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Journal Articles</h2><hr />
{% for post in site.publications reversed %}
  {% if post.category == 'manuscripts' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Conference Papers</h2><hr />
{% for post in site.publications reversed %}
  {% if post.category == 'conferences' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}




