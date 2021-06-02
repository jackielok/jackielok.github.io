---
# Archive design inspired by jameswilson from
# https://talk.jekyllrb.com/t/displaying-archives-design-ideas/2330/4 
# https://www.elementalidad.com/archives

layout: default
title: Archives
permalink: /archives/categories/
---

<nav aria-label="browse archives">
  <strong aria-hidden="true">Browse archives by:</strong>
  <a href="/archives/">year</a> |
  <a href="/archives/categories/" class="active" aria-current="page">(category)</a> |
  <a href="/archives/tags/">tag</a> |
</nav>

{% include by-category.html %}