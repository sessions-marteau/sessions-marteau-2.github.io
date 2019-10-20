---
layout: page
title: Sessions passées
image: 
permalink: /sessions-passes/
tag: 
---

<div class="container">
{%- for post in site.posts -%}
    {% if post.tags.size >= 1 %}
        {% for tag in post.tags %}
            {% if tag == "session" %}
                <div class="row">
                  <div class="col col-12 col-t-12">
                    <div class="row">
                      <article class="article col col-12 col-t-12">
                        <div class="article-box">
                          <div class="article-head">
                            <a href="{{ post.url | prepend: site.baseurl }}" class="article-image" style="background-image: url({{"/img/" | prepend: site.baseurl | append : post.image}})">
                              <div class="image-overlay">
                                <span class="image-overlay-text">{{post.title | slice: 0}}</span>
                              </div>
                            </a>
                          </div>
                          <div class="article-content">
                            <div class="article-info">
                              <div class="article-tag">
                              {% if post.tags.size >= 1 %}
                                {% for tag in post.tags %}
                                <a href="{{ site.baseurl }}/tags#{{tag}}" class="tag">{{ tag }}</a>
                                {% endfor %}
                              {% else %} {% endif %}
                              </div>
                            </div>
                            <h2 class="article-title">
                              <a href="{{ post.url | prepend: site.baseurl }}">{{post.title}}</a>
                            </h2>
                            <p class="article-excerpt">{% if post.description %}{{ post.description | strip_html | truncate: 135 }}{% else %}{{ post.content | strip_html | truncate: 135 }}{% endif %}</p>
                          </div>
                        </div>
                      </article>
                    </div>   
                  </div>
                </div>                
            {% endif %}
        {% endfor %}
    {% endif %}
{% endfor %}
</div>




<!-- <div class="container">
    <div class="row">
      <div class="col col-12 col-t-12">
        <div class="row">
        {%- for post in paginator.posts offset: 1 -%}
          <article class="article col col-12 col-t-6">
            <div class="article-box">
              <div class="article-head">
                <a href="{{ post.url | prepend: site.baseurl }}" class="article-image" style="background-image: url({{"/img/" | prepend: site.baseurl | append : post.image}})">
                  <div class="image-overlay">
                    <span class="image-overlay-text">{{post.title | slice: 0}}</span>
                  </div>
                </a>
              </div>
              <div class="article-content">
                <div class="article-info">
                  <div class="article-tag">
                  {% if post.tags.size >= 1 %}
                    {% for tag in post.tags %}
                    <a href="{{ site.baseurl }}/tags#{{tag}}" class="tag">{{ tag }}</a>
                    {% endfor %}
                  {% else %} {% endif %}
                  </div>
                </div>
                <h2 class="article-title">
                  <a href="{{ post.url | prepend: site.baseurl }}">{{post.title}}</a>
                </h2>
                <p class="article-excerpt">{% if post.description %}{{ post.description | strip_html | truncate: 135 }}{% else %}{{ post.content | strip_html | truncate: 135 }}{% endif %}</p>
              </div>
            </div>
          </article>
        {% endfor %}
        </div>   
      </div>
    </div>
  </div> -->
  
