---
layout: textcontent
---

### Nächstes Treffen

<div class="nextmeetup">
{% for post in site.posts limit: 1 %}
{% if post.title == "" %}
<h1>TBD / 未定</h1>
{% else %}
<a href="{{ post.url }}"><h1>{{ post.title }}</h1></a>
<div class="infohead">
  <span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%Y-%m-%d" }}</span>
  <span><i class="fa fa-clock-o" aria-hidden="true"></i> {{ post.time }}</span>
  <span><i class="fa fa-map-marker" aria-hidden="true"></i> {{ post.place }}</span>
  <span><i class="fa fa-users" aria-hidden="true"></i> {{ post.people }}</span>
</div>
{% endif %}
<div class="postimg"><img src="/assets/img/{{ post.img }}"></div>
{{ post.content }}
{% endfor %}
</div>
<br>
<br>

### Vorherige Treffen

<div>
{% for post in site.posts offset: 1 %}
<p><a href="{{ post.url }}">{{ post.title }}</a> <span class="details">&emsp;<i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%Y-%m-%d" }}&emsp;<i class="fa fa-map-marker" aria-hidden="true"></i> {{ post.place }}<br><i class="fa fa-users" aria-hidden="true"></i> {{ post.people }} : {{ post.compo | join: "・" }}</span></p>

{% endfor %}
<div>
