---
layout: page
title: Archiv
---

<div class="row">        
    <div class="col-sm-6">
        <div class="list-group">

<div class="panel-heading" markdown="1">

### 2015
<ul class="posts">
{% for post in site.posts %}
  {% assign y = post.date | date: "%Y" %}
  {% if y == "2015" %}
  <li>
    <span class="post-date">{{ post.date | date: "%b %-d" }}</span>
    <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
  </li>
  {% endif %}
{% endfor %}
</ul>

### 2014
<ul class="posts">
{% for post in site.posts %}
  {% assign y = post.date | date: "%Y" %}
  {% if y == "2014" %}
  <li>
    <span class="post-date">{{ post.date | date: "%b %-d" }}</span>
    <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
  </li>
  {% endif %}
{% endfor %}
</ul>

</div>

        </div>
    </div>
</div>
