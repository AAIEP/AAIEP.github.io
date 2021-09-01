---
layout: page
title: Guia AAIEP
permalink: /caloiro
comments: false
image: assets/images/back2school.jpg
imageshadow: true
---
Bem vindos, caloiros!

Vai começar agora um novo ciclo das vossas vidas e é com enorme satisfação que a AAIEP está aqui desde o primeiro passo para te ajudar! Neste “guia de sobrevivência'', vamos explicar-te o mais importante, desde dicas para cada cadeira, sítios para estudar até aos sítios mais em conta para almoçar.

Para questões, pensamentos ou sugestões, estamos sempre mais que disponíveis para falar contigo! Se no início for complicado conhecer as nossas caras - não te preocupes, que somos uma casa pequena, e em breve conhecerás todos! - não hesites em [contactar-nos](contactos).

## IEP101: Um guia compreensivo
{% assign posts = site.posts | where:"categories","Guia" %}
{% for post in posts %}
  {% include postbox.html %}
{% endfor %}
