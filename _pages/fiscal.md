---
layout: page
title: Conselho Fiscal
permalink: /fiscal
comments: false
image: assets/images/Fiscal.png
imageshadow: false
---
O Conselho Fiscal da AAIEP é constituído por três elementos, sendo estes o Presidente, o Vice-Presidente e o Secretário. Atualmente, no mandato de 2021/2022, o Conselho Fiscal é composto por:

* **Presidente:** Inês Santareno
* **Vice-Presidente:** Mariana Setra
* **Secretária:** Rafaela Guimarães

Podes contactar o **Conselho Fiscal AAIEP** através do e-mail [fiscal@aaiep.pt](mailto:fiscal@aaiep.pt).

{% assign posts = site.posts | where:"author","fiscal" %}
{% for post in posts %}
  {% include postbox.html %}
{% endfor %}
