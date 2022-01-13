---
layout: default
---

### Blog Posts

<u1>
   {% for post in site.posts %}
      - {{ post.date | date_to_string }}: <a href="{{ post.url }}">{{ post.title }}</a> <br> 
         {{ post.excerpt }}
   {% endfor %}
</u1>


