---
layout: page
title: Guia AAIEP
permalink: /caloiro
comments: false
image: assets/images/ucp_edificio_central.jpg
imageshadow: true
---
Entraste no IEP? Parabéns! Blah blah blah, este texto é temporário. Se encontraste isto podes depois vir cá ver o teu manual do caloiro!

## IEP101: Um guia compreensivo
{% assign posts = site.posts | where:"categories","Guia" %}
{% for post in posts %}
  {% include postbox.html %}
{% endfor %}
