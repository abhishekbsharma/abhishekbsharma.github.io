---
layout: default
title: Insights per Annum
---
<ul class="posts">
  {% for post in site.posts %}
    {% if post.categories contains 'insights' %}
	    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
	    <p class="abstract"> {{ post. abstract }} </p>
	    <br>
	{% endif %}
  {% endfor %}    
</ul>