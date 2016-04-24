---
layout: post
title: "Collected Introductory Multivariate pages"
date: 2015-06-20 00:00
comments: true
categories: container
---

<a name="top"></a>

Articles on the basic principles and practice of Multivariate Statistics - suitable for new-comers and beginners.

<ul>
  {% for post in site.categories.intro %}
	{% if post.url %}
  <li><a href="{{ post.url }}">{{ post.title }}</a></li>
	{% endif %}
  {% endfor %}
</ul>
