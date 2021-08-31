---
layout: page
title: A equipa
permalink: /equipa
comments: false
---
ESCREVER AQUI MAIS ALGUM PARÁGRAFO? MANDEM OPINIÕES PFF

![A equipa](assets/images/equipa2122.png)

Não pode deixar de ser evidente que como alunos do Instituto de Estudos Políticos, temos o dever - senão moral, reputacional - de ser exemplo na conduta e na condução de uma vida académica e associativa tão dinâmica e fervilhante como honesta e honrada. É esse o compromisso da nossa parte; é essa a expectativa que devem ter e pela qual devemos responder.

<div class="video-container">
  <iframe class="video" src="https://www.youtube.com/embed/dQw4w9WgXcQ" allowfullscreen></iframe>
</div>

## Quem somos
<div class="list-authors mt-5">
{% for author in site.authors %}
  {% if author[1].mandato %}
    <div id="{{ author[1].name }}" class="authorbox position-relative pb-5 pt-5 mb-4 mt-4 border">
        <div class="row">
            <div class="wrapavname col-md-3 text-center">
                {% if author[1].gravatar %}
                <img  class="author-thumb" src="https://www.gravatar.com/avatar/{{ author[1].gravatar }}?s=250&d=mm&r=x" alt="{{ author.display_name }}">
                {% else %}
                <img  class="author-thumb" src="{{site.baseurl}}/{{ author[1].avatar }}" alt="{{ author.display_name }}">
                {% endif %}

                <p class="mt-4 mb-0 small text-center">

                    {% if author[1].web %}
                        <a target="_blank" class="d-inline-block mx-1 text-dark" href="{{ author[1].web }}"><i class="fa fa-link"></i></a>
                    {% endif %}

                    {% if author[1].twitter %}
                        <a target="_blank" class="d-inline-block mx-1 text-dark" href="{{ author[1].twitter }}"><i class="fab fa-twitter"></i></a>
                    {% endif %}

                    {% if author[1].email %}
                        <a class="d-inline-block mx-1 text-dark" href="mailto:{{ author[1].email }}"><i class="fa fa-envelope"></i></a>
                    {% endif %}

                </p>

            </div>
            <div class="col-md-9">
                <h3>{{ author[1].display_name }}</h3>
                <p class="mt-3 mb-0">{{ author[1].description }}</p>
            </div>
        </div>
    </div>
  {% endif %}
{% endfor %}
</div>
