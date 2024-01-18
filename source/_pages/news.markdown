---
layout: pages
title: News Archive
permalink: /news/
---
# News Archive:
{% for post in site.posts %}
{% assign currentDate = post.date | date: "%B %Y" %}
### **{{ currentDate }}**

[**{{ post.date | date: "%Y-%m-%d %H:%M"  }}**  
{{ post.title }}]({{ post.url }})
{% endfor %}