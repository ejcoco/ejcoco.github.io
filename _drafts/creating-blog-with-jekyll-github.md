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


## Tema
Como vocês viram acima o GitHub pages trabalha com temas, mas não iremos utilizar uma tema, vamos nos basear em um e modifica-lo, eu vou me basear em um tema do [Samarjeet](https://github.com/thelehhman), o [plainwhite-jekyll](https://github.com/thelehhman/plainwhite-jekyll), 

![tema plainwhite-jekyll](/assets/posts/image08.png){:class="img-print"} 
1. Faça o download do projeto (.zip)
![tema plainwhite-jekyll](/assets/posts/image09.png){:class="img-print"}
Descompacte o conteudo do zip e cole na raiz do seu blog

1.1. Copie
![tema plainwhite-jekyll](/assets/posts/image10.png){:class="img-print"}

1.2. Cole e substitua
![tema plainwhite-jekyll](/assets/posts/image11.png){:class="img-print"}


Após isso execute o comando `bundle exec jekyll serve`
![comando para executar o jekyll](/assets/posts/image12.png){:class="img-print"}

E você verá o seguinte ao acessar o [http://localhost:4000](http://localhost:4000)
![comando para executar o jekyll](/assets/posts/image13.png){:class="img-print"}

Bom, vamos modificar agora para o nosso gosto

## Modificando

Vamos editar o arquivo `_config.yml` na raiz do projeto.

Ele se parece com isso agora:
![_config.yml](/assets/posts/image14.png){:class="img-print"}

Vamos modifica-lo para parecer com isso, removemos as linhas 14-18, e criamos a tag `authors`, que é um array `-` com duas posições, com nossos nomes e fotos e usuarios das redes sociais.
![_config.yml](/assets/posts/image15.png){:class="img-print"}

Vamos agora alterar o arquivo `layouts/default.html`
![layouts/default.html](/assets/posts/image16.png){:class="img-print"}

Ele ficou assim após nossas modificações
![layouts/default.html](/assets/posts/image17.png){:class="img-print"}

Qualquer modificação no arquivo `_config.yml`, precisa que os servidor seja reiniciado, após reiniciar veremos o seguinte:

![_config.yml](/assets/posts/image18.png){:class="img-print"}
