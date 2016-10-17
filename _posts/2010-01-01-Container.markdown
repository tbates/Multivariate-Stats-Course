---
layout: post
title: "Collected Introductory Multivariate pages"
date: 2015-06-20 00:00
comments: true
categories: container
---

<a name="top"></a>

Articles on the basic principles and practice of Multivariate Statistics - suitable for new-comers and beginners.

Core functions in R that you need to memorise.

Core building blocks in statistics that you need to memorize.

Sampling error of the mean:

```splus
 var(df$yourVar)/sqrt(length(df$yourVar))
    
```
Critical statistics are the ratio of an effect size compared to a sampling error. For instance, t = ES / SE

<ul>
  {% for post in site.categories.intro %}
	{% if post.url %}
  <li><a href="{{ post.url }}">{{ post.title }}</a></li>
	{% endif %}
  {% endfor %}
</ul>
