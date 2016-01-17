---
layout: page
title: Apoorv's Blog
tagline: Random thoughts
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
	  <li>
	    <h4 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h4>
	    <p class="post-meta">{{ post.date | date_to_string }}</p>
	    <p class="post-excerpt">
	        {{ post.excerpt | strip_html }}&hellip; 
	        (<a href="{{ post.url }}">Read More</a>)
	    </p>
  </li>
  {% endfor %}
</ul>
