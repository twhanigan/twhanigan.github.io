---
title: "Photos"
collection: Team
type: "archive"
permalink: /Photos/Image_page
date: 2024-08-16
venue: "University of Houston Department of Pharmacological & Pharmaceutical Sciences"
location: "Houston, Texas"
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