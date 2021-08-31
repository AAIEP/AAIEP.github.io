---
layout: page
title: Tutorial do site super secreto
permalink: /top-secret-aaiep-guia-informatico
comments: false
image: https://images.unsplash.com/photo-1603792907191-89e55f70099a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1950&q=80
imageshadow: true
---
Jovem associativista, tens mais de 18 anos? Estás aborrecido e sem nada para fazer? Já alguma vez pensaste para ti próprio/a:

> Ena pá... Queria mesmo ter um site para a minha associação de estudantes, mas o Squarespace e o Wix são caros para o nosso orçamento pequenino!

Se respondeste sim, tenho aqui a tua solução! Fazer um site à borla e pagar apenas a anualidade do domínio que compraste ou então ser mesmo forreta e não pagar nada com o site a correr no [GitHub Pages](https://pages.github.com/) sem domínio. Mas vamos lá com calma que fazer um site não é assim tão fácil como aquela ferramenta toda _fancy_ do Wix e afins que é só arrastar uma coisinha para aqui, uma coisinha para ali, e zás-trás tens um site saído do forno e pronto para chegar a casa antes do jantar. Vamos aqui passo a passo fazer a cena com calma para que não só neste mandato, como no futuro, se saiba como fazer e manter este site sem levar ninguém a dar em louco com o bixo papão da informática.

# Tabela de conteúdos
- [Preciso de...](#preciso-de)
  - [Git](#git)
  - [GitHub](#github)
  - [Atom](#atom)
  - [As coisas Chatas](#as-coisas-chatas)
    - [Ruby](#ruby)
    - [Ruby Gems](#ruby-gems)
    - [Bundler](#bundler)
    - [Jekyll](#jekyll)


## Preciso de...

Além de paciência, de um computador e de uma ligação à internet precisas apenas de mais um milhão de coisas (aproximadamente). Façam por esta ordem idealmente.

### Git

Não confundam isto com o que vem a seguir, mas basta instalarem esta ferramenta através [daqui](https://git-scm.com/), na versão mais recente que aparecer ou a standard, tanto faz.

### GitHub

Apesar da aplicação não ser propriamente necessária para trabalhar com o Git (explico mais à frente), é mais conveniente utilizar a aplicação para o computador do GitHub, disponível [aqui](https://desktop.github.com/). Para funcionar com o GitHub precisam de [ter uma conta](https://github.com/signup) pessoal (nada de andarem a criar contas a torto e a direito estilo "aaiep.geral.20XX/20XY@nãoseiquêmail.com", é horroroso para passar de mandato para mandato), e associarem-se à organização do GitHub [AAIEP](https://github.com/AAIEP) (provavelmente na transição de mandato ou ao longo do mandato, se precisarem de pessoal para fazer isto).

Depois de instalada a aplicação, e já tendo uma conta que está associada à nossa organização, podemos passar para o próximo passo, que é fazer download do site inteiro para o vosso computador. Para fazer isso, abrem o GitHub Desktop, fazem *"File -> Clone repository..."* (ou como quer que isso seja na língua do Camões) e se tudo está bem preparado, devem ter o repositório **AAIEP/AAIEP.github.io** disponível para clonar para o vosso computador. O básico do GitHub é este, mas vamos mais tarde precisar dele para pôr em prática as alterações que fizermos.

### Atom

Isto é mais uma preferência pessoal do que outra coisa, mas no que toca a editores de texto não há nada mais seguro do que o [Atom](https://atom.io/). Podem usar o Notepad, claro, mas é uma complicação enorme estar sempre a saltitar de ficheiro em ficheiro e ter mil e uma janelas abertas. Têm imensas alternativas, como o Visual Studio Code, Sublime Text e o próprio Notepad++, mas se querem uma experiência minimamente agradável e não querem uma interface de utilizador que vos faça sentir como um hacker dos anos 80 com milhares de butões e tudo muito feio recomendo vivamente que se mantenham pelo **Atom**.

### As coisas chatas

Aqui é o que mais vai assustar o pessoal, e peço desde já desculpa se estão a utilizar um Mac, porque isto é mais direcionado para o Windows (sendo que é fazível à mesma, mas com uma ou duas diferenças em certos passos que não sei atualmente). Sim, vão ter de fazer coisas num terminal que afinal sempre vos vai fazer sentir como o tal hacker dos anos 80, mas em vez de butões têm apenas que escrever comandos. Nada vos impede de fazer as coisas no **CMD**, a command line do Windows, mas se é para usar algo do Windows que já vem pré-instalado, mais vale usarem o **Windows PowerShell**, uma CMD mais bonita e com um monte de outras ramificações técnicas que não vale a pena explicar aqui. **NOTA:** Para estas coisas, recomendo que sempre que instalarem algo, assim que terminarem, fechem o terminal e voltem a abrir para fazer o próximo passo.

#### Ruby
O vosso primeiro passo será instalar a linguagem de programação **Ruby** no vosso computador. Ninguém vai estar aqui a programar Ruby, não se preocupem, mas é preciso para correr o resto das coisas. A versão que instalarem do Ruby **deve ser abaixo do 2.7**, portanto recomendo que façam download através [daqui](https://github.com/oneclick/rubyinstaller2/releases/download/RubyInstaller-2.6.8-1/rubyinstaller-devkit-2.6.8-1-x64.exe) e que sigam as instruções base de instalação, ou que procurem pelo *Ruby Installer* (idealmente que diga "x64" se o vosso sistema é de 64 bits, como na maior parte dos casos hoje é) que tenha uma versão abaixo do 2.7 (atualmente recomendo o 2.6.8-1).

#### Ruby Gems
Aqui o guia está bem detalhado na página, e com as vossas ferramentas que instalaram até agora serão capazes de seguir esta instalação. Devem instalar o [Ruby Gems](https://rubygems.org/pages/download) através do link dado. Não indo em grandes detalhes, uma "gem" é um "programa" feito em Ruby que pode ser reutilizado, e é para isso que precisamos desta ferramenta.

#### Bundler
Mais uma coisa chata das "gems", o **Bundler** é uma ferramenta que basicamente, nos agrega todas as "gems" que o site precisa para funcionar. Aqui a coisa é tão simples que basta abrirem a powershell e escrever o seguinte:

```
gem install bundler
```

E ficam com o **Bundler** instalado.

#### Jekyll
A parte final (e mais importante, sendo a razão de termos feito todas estas coisas chatas até agora) é instalar o **Jekyll**. Esta ferramenta é o que nos permite criar o site em si sem percebermos nada (ou muito pouco) de HTML. Assim por alto, isto serve para podermos escrever algo da seguinte maneira:

``` markdown
Olá, o meu nome é **Alberto** *Braz* __Carvalhas__,
e ~~não~~ gosto de fazer [sites](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
```
e obtemos este resultado:

Olá, o meu nome é **Alberto** *Braz* __Carvalhas__, e ~~não~~ gosto de fazer [sites](https://www.youtube.com/watch?v=dQw4w9WgXcQ)

... tudo isto em vez da complicação que é fazer tudo à mão com HTML e CSS.

Portanto, para instalar o Jekyll, basta fazerem como antes:

```
gem install bundler
```

E já está. As partes chatas estão prontas e conseguem seguir o resto deste tutorial mais descansados. A partir de agora é só saberem os básicos de como funcionar com o Jekyll e como é que o projeto (a pasta) está organizada e como é que adicionam ou alteram algo ao site.
