---
layout: post
author: Eduardo
reviewer: Juliane
title: "Criando um blog com jekyll"
date: 2020-02-11 21:00:57 -0300
categories: jekyll blog ejcoco
---

Jekyll + GitHub = blogging

# Jekyll + GitHub

O GitHub possui um serviço chamado de [github pages](https://pages.github.com/) e ele diz que para serviço de blog usamos o Jekyll.

Jekyll é uma engine que disponibiliza um site estático ou blog, utilizando markdown.

## Instalando jekyll

Jekyll é uma [Ruby Gem](https://jekyllrb.com/docs/ruby-101/#gems), logo precisa do ambiente Ruby para funcionar, o site oficial do Jekyll mostra como configurar o ambiente.

1. Para [instalar o ambiente de desenvolvimento Ruby](https://jekyllrb.com/docs/installation/)
2. Com o ambiente configurado digite:

```shell
gem install jekyll bundler
```

3. Agora com o ambiente configurado, nós criamos um blog, digite:

```shell
jekyll new myblog
```

4. Blog criado, entramos na pasta e iniciamos o servidor, digite:

```shell
cd myblog && bundle exec jekyll serve
```

5. Com o servidor levantado ele vai ouvir por padrão no endereço [http://localhost:4000](http://localhost:4000)

Ao acessar o endereço, você verá algo assim:
![pagina padrão](/assets/posts/image01.png){:class="img-print"}

---

## Configurando o GitHub

// falar sobre githubpages

1. Crie uma repositório no github que tenha o sufixo `.github.io`, como na imagem abaixo
   ![criando um repositirio no github](/assets/posts/image02.png){:class="img-print"}

2. Clique em `Settings`
   ![criando um repositirio no github](/assets/posts/image03.png){:class="img-print"}

3. Desça a página até encontrar a seção escrita `GitHub Pages` e clique em `Choose a theme`
   ![criando um repositirio no github](/assets/posts/image04.png){:class="img-print"}

4. Escolhe uma tema qualquer, não faz diferença agora, vamos substituir ele depois
   ![criando um repositirio no github](/assets/posts/image05.png){:class="img-print"}
5. Após escolha do tema, faça commit das alterações
   ![criando um repositirio no github](/assets/posts/image06.png){:class="img-print"}

6. E pronto, seu github pages está online, no caso o nosso é `ejcoco.github.io`, o seu será `<repo>.github.io`
   ![criando um repositirio no github](/assets/posts/image07.png){:class="img-print"}
