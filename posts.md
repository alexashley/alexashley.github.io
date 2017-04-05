---
layout: default
title: All Posts
permalink: /blog/
---

{% for post in site.posts %}	
<h3 class="post-listing"><a href="{{ post.url }}">{{ post.title }}</a></h3>
<p><small><strong>{{ post.date | date: "%B %e, %Y" }}</strong></small></p>			
{% endfor %}