---
layout: page
title: Mohannad Faihan Otaibi
---



<section markdown="1" class="mb-5 p-3 container">
## {{ site.data.db.applications.title }} <br /> <small class="text-muted">{{ site.data.db.applications.description }}</small>   
<ul class="row list-unstyled p-0">
{% for member in site.data.db.applications.data %}
  <li class="col-md-4 pb-3 m-0">
    <div class="row m-0 p-0">
      <a href="{{ member[1].url }}">
        <img height="32" alt="{{ member[0] }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member[1].url }}" class="" /><span class="col-10">{{ member[0] }}</span>
      </a>
    </div>
  </li>
{% endfor %}
</ul>
</section>

<section markdown="1" class="mb-5 p-3 container">
## {{ site.data.db.quotes.title }} <br /> <small class="text-muted">{{ site.data.db.quotes.description }}</small>

{% for member in site.data.db.quotes.data %}
  > {{ member.quote }}
  > <small><cite>{{ member.author }}</cite></small>

{% endfor %}
</section>

<section markdown="1" class="mb-5 p-3 container">
## {{ site.data.db.bookmarks.title }} <br /> <small class="text-muted">{{ site.data.db.bookmarks.description }}</small>
<ul class="row list-unstyled p-0">
{% for member in site.data.db.bookmarks.data %}
  <li class="col-md-4 pb-3 m-0">
    <div class="row m-0 p-0">
      <a href="{{ member.url }}">
        <img height="16" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
      </a>
    </div>
  </li>
{% endfor %}
</ul>
</section>

<section markdown="1" class="mb-5 p-3 container">
## {{ site.data.db.organizations.title }} <br /> <small class="text-muted">{{ site.data.db.organizations.description }}</small>
<ul class="row list-unstyled p-0">
{% for member in site.data.db.organizations.data %}
  <li class="col-md-3 pb-3 m-0">
    <div class="row m-0 p-0">
      <img height="32" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
    </div>
  </li>
{% endfor %}
</ul>
</section>

<section markdown="1" class="mb-5 p-3 container">
## {{ site.data.db.accomplishments.title }} <br /> <small class="text-muted">{{ site.data.db.accomplishments.description }}</small>
<ul class="row list-unstyled p-0">
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
</section>

<section markdown="1" class="mb-5 p-3 container">
## {{ site.data.db.languages.title }} <br /> <small class="text-muted">{{ site.data.db.languages.description }}</small>
<ul class="list-inline p-0">
{% for member in site.data.db.languages.data %}
  <li class="pb-4 pl-0 pr-4 m-0 list-inline-item">

      {% if member.svg %}
      <a href="{{ member.url }}" style="font-size:48px;">
          <i class="{{ member.svg }}"></i>
        </a>
      {% else %}
        <a href="{{ member.url }}" style="font-size:48px;">
          <img height="48" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="grayscale" />
        </a>
      {% endif %}


  </li>
{% endfor %}
</ul>
</section>

<section markdown="1" class="mb-5 p-3 container">
## {{ site.data.db.standards.title }} <br /> <small class="text-muted">{{ site.data.db.standards.description }}</small>
<ul class="row list-unstyled p-0">
{% for member in site.data.db.standards.data %}
  <li class="col-md-4 pb-3 m-0">
    <div class="row m-0 p-0">
      <img height="32" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
    </div>
  </li>
{% endfor %}
</ul>
</section>

<section markdown="1" class="mb-5 p-3 container">
## {{ site.data.db.games.title }} <br /> <small class="text-muted">{{ site.data.db.games.description }}</small>
<ul class="row list-unstyled p-0">
{% for member in site.data.db.games.data %}
  <li class="col-md-6 pb-3 m-0">
    <div class="row m-0 p-0">
      <img height="32" alt="{{ member.title }}" src="https://i.olsh.me/icon?size=80..120..200&url={{ member.url }}" class="" /><span class="col-10">{{ member.title }}</span>
    </div>
  </li>
{% endfor %}
</ul>
</section>

<section markdown="1" class="mb-5 p-3 container">
## {{ site.data.db.locations.title }} <br /> <small class="text-muted">{{ site.data.db.locations.description }}</small>
<div id="map" style="height:400px;"></div>
</section>

<script>
// Initialize and add the map
function initMap() {
  var uluru = {lat: 47.142198, lng: 1.080505};
  var map = new google.maps.Map(document.getElementById('map'), {
    zoom: 2,
    center: uluru,
    clickableIcons: false,
    disableDefaultUI: true,
    });

    var marker;

    {% for member in site.data.db.locations.data %}
      marker = new google.maps.Marker({
        position: new google.maps.LatLng({{ member.lat }}, {{ member.lng }}),
        map: map
      });
    {% endfor %}

}
</script>


<!-- use a serverless form -->
<section markdown="1" class="mb-5 p-3 container">
## Contact Me <br /> <small>for Projects, Questions, or simply saying Hi!</small>
<!-- a serverless contact us form -->
<form class="needs-validation" action="https://formsubmit.co/mohannad.otaibi+webform@gmail.com" type="post" novalidate>
  <input type="hidden" name="_subject" value="New Message from Mohannadotaibi.com!" />
  <input type="text" name="_honey" style="display:none" />
  <input type="hidden" name="_captcha" value="false" />
  <input type="hidden" name="_template" value="box" />

  <div class="form-group pb-2 border-bottom">
    <input type="text" class="form-control form-control-lg border-0 rounded-0" id="yourName" name="yourName" placeholder="Name" required>
    <div class="invalid-feedback">
      Please write a name
    </div>
  </div>

  <div class="form-group pb-2 border-bottom">
    <input type="email" class="form-control form-control-lg border-0  rounded-0" id="email" name="email" placeholder="Email Address" required>
    <div class="invalid-feedback">
      Please write your email.
    </div>
  </div>



  <div class="form-group pb-2 border-bottom">
    <textarea class="form-control form-control-lg border-0 rounded-0" id="message" name="message" rows="5" placeholder="Your Message" required></textarea>
    <div class="invalid-feedback">
      Please type a message
    </div>
  </div>

  <div class="form-group">
    <button type="submit" class="btn btn-success btn-lg btn-block">Send <i class="fas fa-paper-plane"></i></button>
  </div>

</form>
</section>
<script>
  // Example starter JavaScript for disabling form submissions if there are invalid fields
  (function() {
    'use strict';
    window.addEventListener('load', function() {
      // Fetch all the forms we want to apply custom Bootstrap validation styles to
      var forms = document.getElementsByClassName('needs-validation');
      // Loop over them and prevent submission
      var validation = Array.prototype.filter.call(forms, function(form) {
        form.addEventListener('submit', function(event) {
          if (form.checkValidity() === false) {
            event.preventDefault();
            event.stopPropagation();
          }
          form.classList.add('was-validated');
        }, false);
      });
    }, false);
  })();
</script>


<!-- https://i.olsh.me/icon?size=80..120..200&url={{ member[1].url }} -->
<!-- http://f3.allesedv.com/16/{{ member[1].url }} -->
