---
layout: default
title: Gallery
permalink: /gallery/
---

<h1>Gallery</h1>

<div style="display: flex; flex-wrap: wrap; gap: 20px;">
  {% for item in site.gallery %}
    <div style="border: 1px solid #ddd; padding: 15px; width: 600px; text-align: left;">
      <a href="{{ item.url }}">
        <img src="{{ item.image }}" alt="{{ item.title }}" style="max-width: 100%;">
      </a>
      <p style="font-size: 15px; font-style: italic;">{{ item.title }}</p> 
      <p style="font-size: 15px; color: #666;">{{ item.description }}</p> 
    </div>
  {% endfor %}
</div>
