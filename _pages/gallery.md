---
layout: default
title: Gallery
permalink: /gallery/
---

<h1>Gallery</h1>

<div style="display: grid; grid-template-columns: repeat(auto-fill, 710px); gap: 20px;">
  {% for item in site.gallery %}
    <div 
      style="border: 1px solid #ddd; padding: 15px; text-align: left;
             grid-row: 
             {% if item.span_three_lines %}span 3;
             {% elsif item.span_two_lines %}span 2;
             {% else %}auto;{% endif %};">
      
      <!-- Item Title -->
      <h2 style="font-size: 18px; font-weight: bold; margin-bottom: 5px;">{{ item.title }}</h2>
      
      <!-- Item Description -->
      <p style="font-size: 16px; color: #666; margin-bottom: 16px;">{{ item.description }}</p>

      <!-- Media items -->
      {% if item.media %}
        {% for media in item.media %}
          <figure style="margin-bottom: 10px; text-align: center;">
            {% if media.type == "image" %}
              <img src="{{ media.src }}" alt="{{ media.alt }}" style="max-width: 100%;">
            {% elsif media.type == "video" %}
              <video controls loop style="max-width: 100%;">
                <source src="{{ media.src }}" type="video/{{ media.format }}">
                Your browser does not support the video tag.
              </video>
            {% endif %}
            {% if media.caption %}
              <figcaption style="font-size: 16px; font-style: italic; color: #666; margin-top: 5px; text-align: left;">
                {{ media.caption }}
              </figcaption>
            {% endif %}
          </figure>
        {% endfor %}
      {% endif %}
    </div>
  {% endfor %}
</div>

