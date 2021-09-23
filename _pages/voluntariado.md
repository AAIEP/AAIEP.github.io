---
layout: page
title: Bolsa de voluntariado AAIEP
permalink: /voluntariado
comments: false
image: assets/images/voluntariado.jpg
imageshadow: false
---
A bolsa de voluntariado consiste num projeto destinado a todos os associados, com propostas de diversas associações de voluntariado para poderes fazer a diferença numa delas. Aqui vais poder usufruir de um acesso mais facilitado a estas instituições e consequentemente ajudar aqueles que mais precisam!

<!-- Posts Index
================================================== -->
{% assign posts = site.posts | where:"author","voluntariado" %}
{% for post in posts %}
  {% include postbox.html %}
{% endfor %}
