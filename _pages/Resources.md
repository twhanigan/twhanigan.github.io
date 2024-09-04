---
layout: archive
title: "Resources"
collection: Resources
permalink: /Resources/
#venue: "University of Houston Department of Pharmacological & Pharmaceutical Sciences"
#date: 2024-08-16
#location: "Houston, Texas"
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.Resources reversed %}
  {% include archive-single.html %}
{% endfor %}
