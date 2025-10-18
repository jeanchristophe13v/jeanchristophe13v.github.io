---
layout: section
title: articles
permalink: /articles
---
{% assign published_articles = site.articles | where: "published", true | reverse %}
{% include sections/last_post.html last_post=published_articles.first %}
{% include sections/items_except_last.html items=published_articles %}
