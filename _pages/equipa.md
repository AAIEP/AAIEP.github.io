---
layout: page
title: A equipa
permalink: /equipa
comments: false
image: assets/images/equipa2122.png
imageshadow: true
---
Não pode deixar de ser evidente que como alunos do Instituto de Estudos Políticos, temos o dever - senão moral, reputacional - de ser exemplo na conduta e na condução de uma vida académica e associativa tão dinâmica e fervilhante como honesta e honrada. É esse o compromisso da nossa parte; é essa a expectativa que devem ter e pela qual devemos responder.

## Quem somos
<div class="list-authors mt-5">
{% for author in site.authors %}
  {% if author[1].mandato %}
    <div id="{{ author[1].name }}" class="authorbox position-relative pb-5 pt-5 mb-4 mt-4">
        <div class="row">
            {% if author[1].avatar %}
            <div class="wrapavname col-md-3 text-center">
                <img  class="author-thumb" src="{{site.baseurl}}/{{ author[1].avatar }}" alt="{{ author.display_name }}">
            </div>
            {% endif %}
            <div class="col-md-9">
                <h3>{{ author[1].display_name }}</h3>
                <p class="mt-3 mb-0">{{ author[1].description }}</p>
            </div>
        </div>
    </div>
  {% endif %}
{% endfor %}
</div>
