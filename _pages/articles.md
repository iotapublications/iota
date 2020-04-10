---
layout: section
title: Articles
permalink: /articles
---
{% assign articles = (site.documents | where: "layout","post") %}
{% include sections/last_post.html last_post=articles.last%}
{% include sections/items_except_last.html items=articles%}
