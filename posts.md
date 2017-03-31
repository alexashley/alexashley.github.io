---
---
{% for post in site.posts %}	
    ##[{{ post.url }}]({{ post.title }})
    {{ post.date | date: "%B %e, %Y" }}	
{% endfor %}