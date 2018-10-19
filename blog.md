---
layout: page
title: Blog
permalink: /blog/
---

"You must have a blog, right?"
-- some dude, 2015

I write rarely, so don't worry.

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
{% endfor %}
