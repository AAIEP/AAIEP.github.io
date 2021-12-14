---
layout: post
title:  "Reviews das opcionais"
author: direcao
tags: [ 2021/2022 ]
image: https://lexrexcommunications.com/wp-content/uploads/2018/10/shutterstock_683543383.jpg
comments: false
---

# Primeiro Semestre

{% assign s1 = site.posts | where:"semestre",1 %}
{% for post in s1 %}
  {% include postbox.html %}
{% endfor %}

# Segundo Semestre

{% assign s2 = site.posts | where:"semestre",2 %}
{% for post in s2 %}
  {% include postbox.html %}
{% endfor %}
