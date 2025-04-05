---
title: Home
layout: home
nav_order: 1
---
## Welcome to this communal recipe repository. 

I'm still figuring out a solution for tagging and sorting recipes but until then the search function works just fine.
I'm planning on adding a dataview table here of recipes links in the future. For now I have a list of tag links.


<ul>
  {% for post in site.pages %}
  {% if post.title contains "Tag" %}
  
  
  <li><a class="page" href="{{ post.url }}">{{ post.title }}</a></li>
  {% endif %}
  {% endfor %}
</ul>
