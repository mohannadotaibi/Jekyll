---
layout: page
title: Mohannad Faihan Otaibi
---

---

## {{ site.data.db.social_links.title }}<br /> <small>{{ site.data.db.social_links.description }}</small>
---

### General
<ul class="list-inline mb-5">
{% for member in site.data.db.social_links.data.general %}
  <li class="list-inline-item">
    <a href="{{ member.url }}">
      <img height="32" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" />
    </a>
  </li>
{% endfor %}
</ul>

---

### Technical Social Media
<ul class="list-inline mb-5">
{% for member in site.data.db.social_links.data.technical %}
  <li class="list-inline-item">
    <a href="{{ member.url }}">
      <img height="32" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" />
    </a>
  </li>
{% endfor %}
</ul>



## {{ site.data.db.applications.title }} <br /> <small>{{ site.data.db.applications.description }}</small>
---

<ul class="list-inline mb-5">
{% for member in site.data.db.applications.data %}
  <li class="list-inline-item mb-3">
    <a href="{{ member[1].url }}"><img height="32" alt="{{ member[0] }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member[1].url }}" /></a>
  </li>
{% endfor %}
</ul>



## {{ site.data.db.quotes.title }} <br /> <small>{{ site.data.db.quotes.description }}</small>
---

{% for member in site.data.db.quotes.data %}
  > {{ member.quote }}
  > <small><cite>{{ member.author }}</cite></small>

{% endfor %}
<div class="mb-5"></div>


## {{ site.data.db.bookmarks.title }} <br /> <small>{{ site.data.db.bookmarks.description }}</small>
---

<ul class="row list-unstyled p-0 mb-5">
{% for member in site.data.db.bookmarks.data %}
  <li class="col-md-6 pb-3 m-0">
    <div class="row m-0 p-0">
      <img height="16" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span class="col-11">{{ member.title }}</span>
    </div>
  </li>
{% endfor %}
</ul>

## {{ site.data.db.organizations.title }} <br /> <small>{{ site.data.db.organizations.description }}</small>
---

<ul class="row list-unstyled p-0 mb-5">
{% for member in site.data.db.organizations.data %}
  <li class="col-md-6 pb-3 m-0">
    <div class="row m-0 p-0">
      <img height="32" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
    </div>
  </li>
{% endfor %}
</ul>


## {{ site.data.db.accomplishments.title }} <br /> <small>{{ site.data.db.accomplishments.description }}</small>
---

<ul class="row list-unstyled p-0 mb-5">
{% for member in site.data.db.accomplishments.data %}
  <li class="col-md-12 pb-3 m-0">
    <div class="row m-0 p-0">
    <a href="{{ member.url }}">
      <img height="32" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span {% if member.arabic %}dir="rtl" {% endif %}class="col-10">{{ member.title }}</span>
    </a>

    </div>
  </li>
{% endfor %}
</ul>


## {{ site.data.db.languages.title }} <br /> <small>{{ site.data.db.languages.description }}</small>
---

<ul class="row list-unstyled p-0 mb-5">
{% for member in site.data.db.languages.data %}
  <li class="col-md-4 pb-3 m-0">
    <div class="row m-0 p-0">
      <img height="16" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
    </div>
  </li>
{% endfor %}
</ul>


## {{ site.data.db.standards.title }} <br /> <small>{{ site.data.db.standards.description }}</small>
---

<ul class="row list-unstyled p-0 mb-5">
{% for member in site.data.db.standards.data %}
  <li class="col-md-6 pb-3 m-0">
    <div class="row m-0 p-0">
      <img height="32" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
    </div>
  </li>
{% endfor %}
</ul>


## {{ site.data.db.games.title }} <br /> <small>{{ site.data.db.games.description }}</small>
---

<ul class="row list-unstyled p-0 mb-5">
{% for member in site.data.db.games.data %}
  <li class="col-md-6 pb-3 m-0">
    <div class="row m-0 p-0">
      <img height="32" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
    </div>
  </li>
{% endfor %}
</ul>



<!-- https://i.olsh.me/icon?size=80..120..200&url={{ member[1].url }} -->
<!-- http://f3.allesedv.com/16/{{ member[1].url }} -->
