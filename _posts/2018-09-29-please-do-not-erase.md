---
layout: post
title: Please Do Not Erase
---

<head>
  <script src="/js/jquery-1.11.2.min.js"></script>
  <script>
    let words = {
    }

    function googleImage() {
      console.log("googling image")
    }

    $("h1").text("Jquery works")
    $("p").text("swap")
  </script>
</head>

<div>
  <h1>Test 3</h1>
  <p>another test</p>
  {% for image in site.static_files %}
    {% if image.path contains 'XXXimg/project1' %}
      <img src="{{ site.baseurl }}{{ image.path }}" alt="image" />
    {% endif %}
  {% endfor %}
</div>
