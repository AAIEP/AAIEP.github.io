---
layout: page
title: Parcerias
permalink: /parceiros
comments: false
---
A AAIEP orgulha-se de trabalhar com os seus parceiros! Para saberes mais sobre como tu beneficias destas parcerias, lê abaixo sobre cada uma delas.

Se é uma instituição ou empresa terceira e deseja colaborar com a AAIEP por favor contacte-nos através de [parcerias@aaiep.pt](mailto:parcerias@aaiep.pt).

{% assign posts = site.posts | where:"categories","Parceria" %}
{% for post in posts %}
  {% include postbox.html %}
{% endfor %}
