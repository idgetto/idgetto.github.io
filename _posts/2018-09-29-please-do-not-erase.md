---
layout: post
title: Please Do Not Erase
---

<head>
  <script>
    let words = {
      'IMG_2141':
    }

    function googleImage() {
      console.log("googling image")
    }
  </script>
</head>

<div>
  <h1>Test</h1>

  <!-- <img src="{{ site.baseurl }}/img/project1/IMG_2142.JPG" onclick="googleImage()" /> --!>
  {% for image in site.static_files %}
    {% if image.path contains 'images/project1' %}
      <img src="{{ site.baseurl }}{{ image.path }}" alt="image" />
    {% endif %}
  {% endfor %}
</div>
