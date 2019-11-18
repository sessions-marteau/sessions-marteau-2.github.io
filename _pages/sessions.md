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
	
	

La prochaine session d'ecoute sera le 29 novembre 2019

AVEC Sam Shalabi

Les portes ouvrent à 18:30

PROGRAMME (à partir de 19h):

Le public pourra compter sur le travail de sélection du commissaire invité Sam Shalabi, compositeur et improvisateur canado-égyptien, installé à Montréal. Ayant débuté dans le punk rock à la fin des années 70, son travail a évolué pour devenir une fusion de musique expérimentale et moderne qui incorpore la musique arabe traditionnelle; le shaabi, le noise, la musique classique, le texte, l'improvisation et le jazz.

Le thème de cette session est "la musique psychédélique avant la psychedelia", il sagit de la musique qui émerge à partir de la conscience et qui a influencé la musique psychédélique.

Programme et durée sujet à changement sans préavis

Durée 120 minutes

Réservation requise sur Eventbrite, places limités. https://www.eventbrite.ca/e/sessions-decoutelistening-sessions-marteau-3-sam-shalabi-tickets-76809103095?fbclid=IwAR3zodre6bkDAszi7jh7n071LywtaHmqB0D7UPfwJ7pjjO8kwkRchyjGPzo

Évènement Facebook: https://www.facebook.com/events/2463061277300783/
