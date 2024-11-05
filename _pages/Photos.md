---
layout: single
title: "Photos"
permalink: /Photos/
author_profile: true
---
![Alt text](/images/Lab_Photos/20241030_174452.png)

# Image Gallery

<div class="gallery">
  {% assign images = site.static_files | where: "path", "/images/Lab_Photos/" %}
  {% for image in images %}
    <div class="gallery-item">
      <img src="{{ image.path | relative_url }}" alt="Image">
    </div>
  {% endfor %}
</div>
