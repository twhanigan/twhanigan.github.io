---
title: "Photos"
layout: default
permalink: /Photos/Image_page
---

# Image Gallery

<div class="gallery">
  {% assign images = site.static_files | where: "path", "/images/Lab_Photos/" %}
  {% for image in images %}
    <div class="gallery-item">
      <img src="{{ image.path | relative_url }}" alt="Image">
    </div>
  {% endfor %}
</div>