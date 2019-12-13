---
layout: sessions
title: Sessions d'écoute passes
image: 
permalink: /sessions/
tag: session
---

<div class="container">
	<div class="row">
    	{%- for post in paginator.posts offset: 1 -%}
        <span class="image-overlay-text">{{post.title | slice: 0}}</span>
        <h2 class="article-title"><a href="{{ post.url | prepend: site.baseurl }}"></a></h2>
        {% endfor %}
    </div>
</div>    

<!-- <div class="container">
	<div class="row">
	{% if site.posts.size > 0 %}
		{%- for post in paginator.posts -%}
		{% if forloop.index <= 1 %}
		<div class="col col-12">
			<article class="article-first">
				<div class="article-image-first" style="background-image: url({{"/img/" | prepend: site.baseurl | append : post.image}})">
					<div class="article-content-first">
						<div class="article-tag">
						{% if post.tags.size >= 1 %}
							{% for tag in post.tags %}
							<a href="{{ site.baseurl }}/tags#{{tag}}" class="tag">{{ tag }}</a>
							{% endfor %}
						{% else %} {% endif %}
						</div>
						<h2 class="article-title"><a href="{{ post.url | prepend: site.baseurl }}"></a></h2>
						<p class="article-excerpt">{% if post.description %}{{ post.description | strip_html | truncate: 163 }}{% else %}{{ post.content | strip_html | truncate: 163 }}{% endif %}</p>
					</div>
				</div>
			</article> 
		</div>
		{% endif %}

		{% endfor %}
	{% endif %} -->
	
