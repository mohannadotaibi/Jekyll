---
layout: page
title: Mohannad Faihan Otaibi
---

<!-- Applications -->
<section markdown="1" class="my-2 px-1 py-3 my-md-5 px-md-3 py-md-5">
<div class="container">
<h2>{{ site.data.db.applications.title }} <small class="text-muted">{{ site.data.db.applications.description }}</small></h2>
<hr class="my-4" />
<div class="row g-3">
    {% for member in site.data.db.applications.data %}
    <div class="col-12 col-md-3 mini-link">
        <a rel="nofollow" target="_blank" href="{{ member[1].url }}">
            <img height="32" alt="{{ member[0] }}" src="{{site.favicon_grabber}}{{ member[1].url }}" class="" /><span class="col-10">{{ member[0] }}</span>
        </a>
    </div>
    {% endfor %}
</div>
</div>
</section>

<!-- Quotes -->
<section markdown="1" class="my-2 px-1 py-3 my-md-5 px-md-3 py-md-5">
<div class="container">
<h2>{{ site.data.db.quotes.title }} <small class="text-muted">{{ site.data.db.quotes.description }}</small></h2>
<hr class="my-4" />
{% for member in site.data.db.quotes.data %}

<figure class="mb-4">
  <blockquote class="blockquote ps-3">
    <p>{{ member.quote }}</p>
  </blockquote>
  <figcaption class="blockquote-footer">
    <cite title="Source Title">{{ member.author }}</cite>
  </figcaption>
</figure>

{% endfor %}
</div>
</section>

<!-- Bookmarks -->
<section markdown="1" class="my-2 px-1 py-3 my-md-5 px-md-3 py-md-5">
<div class="container">
<h2>{{ site.data.db.bookmarks.title }} <small class="text-muted">{{ site.data.db.bookmarks.description }}</small></h2>
<hr class="my-4" />
<div class="row g-3">
    {% for member in site.data.db.bookmarks.data %}
    <div class="col-12 col-md-4 mini-link">
        <a rel="nofollow" target="_blank" href="{{ member.url }}">
            <img height="32" alt="{{ member.title }}" src="{{site.favicon_grabber}}{{ member.url }}" class="" />
            <span class="col-10">{{ member.title }}</span>
        </a>
    </div>
    {% endfor %}
</div>
</div>
</section>

<!-- Organizations -->
<section markdown="1" class="my-2 px-1 py-3 my-md-5 px-md-3 py-md-5">
<div class="container">
<h2>{{ site.data.db.organizations.title }} <small class="text-muted">{{ site.data.db.organizations.description }}</small></h2>
<hr class="my-4" />
<div class="row g-3">
    {% for member in site.data.db.organizations.data %}
    <div class="col-12 col-md-3 mini-link">
        <a>
            <img height="32" alt="{{ member.title }}" src="{{site.favicon_grabber}}{{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
        </a>
    </div>
    {% endfor %}
</div>
</div>
</section>

<!-- Things Done -->
<section markdown="1" class="my-2 px-1 py-3 my-md-5 px-md-3 py-md-5">
<div class="container">
<h2>{{ site.data.db.accomplishments.title }} <small class="text-muted">{{ site.data.db.accomplishments.description }}</small></h2>
<hr class="my-4" />
<div class="row g-3">
    {% for member in site.data.db.accomplishments.data %}
    <div class="col-12 col-md-6 mini-link">
        <a rel="nofollow" target="_blank" href="{{ member.url }}">
            <img height="32" alt="{{ member.title }}" src="{{site.favicon_grabber}}{{ member.url }}" class="" /><span {% if member.arabic %}dir="rtl" {% endif %} class="col-10">{{ member.title }}</span>
        </a>
    </div>
    {% endfor %}
</div>
</div>
</section>

<section markdown="1" class="my-2 px-1 py-3 my-md-5 px-md-3 py-md-5">
<div class="container">
<h2>{{ site.data.db.languages.title }} <small class="text-muted">{{ site.data.db.languages.description }}</small></h2>
<hr class="my-4" />
<div class="row g-3">
    {% for member in site.data.db.languages.data %}
    <div class="col-12 col-md-2 mini-link">
        <a rel="nofollow" target="_blank" href="{{ member.url }}">
            {% if member.svg %}
                <img height="18" alt="{{ member.title }}" src="{{site.favicon_grabber}}{{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
                <!--<i class="{{ member.svg }}"></i>-->
            {% else %}
                <img height="18" alt="{{ member.title }}" src="{{site.favicon_grabber}}{{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
            {% endif %}
        </a>
    </div>
    {% endfor %}
</div>
</div>
</section>

<section markdown="1" class="my-2 px-1 py-3 my-md-5 px-md-3 py-md-5">
<div class="container">
<h2>{{ site.data.db.standards.title }} <small class="text-muted">{{ site.data.db.standards.description }}</small></h2>
<hr class="my-4" />
<div class="row g-3">
    {% for member in site.data.db.standards.data %}
    <div class="col-12 col-md-4 mini-link">
        <a rel="nofollow" target="_blank" href="{{ member.url }}">
            <img height="32" alt="{{ member.title }}" src="{{site.favicon_grabber}}{{ member.url }}" class="" /><span {% if member.arabic %}dir="rtl" {% endif %} class="col-10">{{ member.title }}</span>
        </a>
    </div>
    {% endfor %}
</div>
</div>
</section>

<section markdown="1" class="my-2 px-1 py-3 my-md-5 px-md-3 py-md-5">
<div class="container">
<h2>{{ site.data.db.games.title }} <small class="text-muted">{{ site.data.db.games.description }}</small></h2>
<hr class="my-4" />
<div class="row g-3">
    {% for member in site.data.db.games.data %}
    <div class="col-12 col-md-4 mini-link">
        <a rel="nofollow" target="_blank" href="{{ member.url }}">
            <img height="32" style="height:32px;" alt="{{ member.title }}" src="{{site.favicon_grabber}}{{ member.url }}" class="" /><span {% if member.arabic %}dir="rtl" {% endif %} class="col-10">{{ member.title }}</span>
        </a>
    </div>
    {% endfor %}
</div>
</div>
</section>

<!-- Places -->
<section markdown="1" class="mt-2 pt-3 mt-md-5 pt-md-5">
<div class="container">
<h2 class="mb-4">{{ site.data.db.locations.title }} <small class="text-muted">{{ site.data.db.locations.description }}</small></h2>
</div>
<div id="map" class="shadow-sm" style="height:600px;"></div>
</section>
