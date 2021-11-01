---
layout: archive
permalink: /blog/
---

{% assign posts = site.posts | sort: date | reverse %}

{% for post in posts %}  
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  

  <a href="{{ post.url }}">
    <img src="{{ site.url }}{{ site.baseurl }}{{ post.post_thumbnail }}" alt="" class="align-left thumbnail-img">
  </a> 
  
  <div>{{ post.excerpt }}</div>
  
  <div class="clear"></div>
  
  <hr>
{% endfor %}  