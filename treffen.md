---
layout: textcontent
---

### Nächstes Treffen

<div class="nextmeetup">
{% for post in site.posts limit: 1 %}
<a href="{{ post.url }}"><h1>{{ post.title }}</h1></a>
<div class="infohead">
  <span>[</span>
  <span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%Y-%m-%d" }}</span>
  <span><i class="fa fa-clock-o" aria-hidden="true"></i> {{ post.time }}</span>
  <span><i class="fa fa-map-marker" aria-hidden="true"></i> {{ post.place }}</span>
  <span><i class="fa fa-users" aria-hidden="true"></i> {{ post.people }}</span>
  <span>]</span>
</div>
<div class="postimg"><img src="/assets/img/{{ post.img }}"></div>
{{ post.content }}
{% endfor %}
</div>
<br>
<br>

### Vorherige Treffen

<div>
{% for post in site.posts offset: 1 %}
<p><a href="{{ post.url }}">{{ post.title }}</a> <span class="details">( <i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%Y-%m-%d" }} / <i class="fa fa-map-marker" aria-hidden="true"></i> {{ post.place }} / <i class="fa fa-users" aria-hidden="true"></i> {{ post.people }} )</span></p>

{% endfor %}
<div>
