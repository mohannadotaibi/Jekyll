---
layout: page
title: Bootstrap 4 Github Pages
---
{% for member in site.data.db.social_links.data.general %}
  * [{{member.title}}]({{member.url}}) - {{member}}
{% endfor %}
