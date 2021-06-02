---
# Archive design inspired by jameswilson from
# https://talk.jekyllrb.com/t/displaying-archives-design-ideas/2330/4 
# https://www.elementalidad.com/archives

layout: page
title: Archives
permalink: /archives/
---

<nav aria-label="browse archives">
  <strong aria-hidden="true">Browse archives by:</strong>
  <a href="/archives/" class="active" aria-current="page">(year)</a> |
  <a href="/archives/categories/">category</a> |
  <a href="/archives/tags/">tag</a> |
</nav>

{% include by-year.html %}
