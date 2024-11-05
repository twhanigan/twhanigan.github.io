---
layout: single
title: "Photos"
permalink: /Photos/
author_profile: true
---

# Image Gallery

<div class="gallery">
  {% assign images = site.static_files | where_exp: "file", "file.path contains '/images/Lab_Photos/' and file.ext in '.jpg, .jpeg, .png'" %}
  {% for image in images %}
    <div class="gallery-item">
      <img src="{{ image.path | relative_url }}" alt="Image">
    </div>
  {% endfor %}
</div>
