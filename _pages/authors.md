---
layout: section
title: Authors
permalink: /authors
---
{% for author in site.authors %}
<div class="container border-bottom">
  <div class="card my-3 border-0">
    <div class="row no-gutters">
      <div class="col-md-8">
        <div class="card-body">
          <a href="{{ author.url }}">
          	<h5 class="card-title">{{ author.name }}</h5>
          </a>
          <p class="card-text">{{ author.content | markdownify }}</p>
        </div>
      </div>
      <div class="col-md-2">
        <img src="{{author.image}}" class="card-img" alt="...">
      </div>
    </div>
  </div>
</div>
{% endfor %}
