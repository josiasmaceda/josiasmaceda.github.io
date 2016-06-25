---
layout: post
title: "Jekyll - O que é, para que serve?"
date: 2016-06-10 18:38:00
comments: true
disqus: true
author: josiasmaceda
categories: web jekyll
---

![Jekyll](https://jekyllrb.com/img/logo-2x.png)

Hello! Já ouvi falar do jekyll?  

Jekyll é um gerador de sites estáticos desenvolvido em Ruby, sendo muito utilizado para a criação de Blogs, sim Blogs, este blog foi desenvolvido utilizando Jekyll, o que achou legal né :). A grande vantagem é de não necessitar de banco de dados ou servidor backend para armazenar os posts no caso de um Blog, outro ponto positivo é que o site vai ser todo estático, logo o carregamento será muito mais rápido que outras ferramentas de criação de blogs como o Wordpress. 

O **[Jekyll](http://jekyllrb.com/ "Clique aqui e acesse o site do Jekyll")** utiliza a ferramenta Liquid para a criação de templates, e o YAML para o armazenamento de variáveis, e o mais interessante ele utiliza o Markdown para a formatação de textos, neste caso POSTs do blog. Para começar a brincar com ele :) comece instalando ele, para saber como instalar veja o post **[Instalando o Jekyll](https://josiasmaceda.com.br/web/jekyll/2016/06/11/instalando-o-jekyll.html "clique aqui")** onde detalho como instalar e iniciar ele pela primeira vez. 


>### Como funciona

`Go go go....`  

Quando você cria um projeto no Jekyll ele cria uma estrutura de diretórios e arquivos dos quais serão a base para gerar o Site posteriormente com apenas uma linha de comando.  

**Os principais dirétorios são:**

 `_includes` onde são colocados todos os templates/html/arquivos que se repetem no site como footer.html, head.html.

`_layouts` ficam armazenados layouts de páginas como exemplo post.html no qual serve como o modelo de página para apresentar os posts do blog.

`_posts` aqui você vai encontrar os posts que serão escritos no formato MarkDown e o Jekyll se encarregará de gerar o html e o post configurado em seu blog. Aqui a extensão do arquivo pode ser `.md` ou `.markdown`.

`_site` e por fim a pasta que contém o build do projeto, ou seja, a versão final estática do site (html+css+javascript) que é gerada pelo Jekyll.

**Os principis arquivos são:**

`_config.yml` arquivo que contém as configurações globais do projeto.

>### YAML

No Jekyll o YAML é conhecido como **front-matter**. Um bloco de YAML é identificado por três traços no começo e fim de uma instrução. No Exemplo abaixo é definido que a variável layout vai utilizar o template default.html, e a title vai definir o título da página.

```html
---
layout: default
title: Post com jekyll
---
```

>### Liquid

Você observou que utilizando o YAML definimos o nome da variável title, agora vamos utilizar ela utilizando Liquid. Para utilizar basta colocar ``{{page.title}}`` em meio ao seu html para que o Jekyll substitua a instrução pela que foi definida na declaração da variável. Veja o exemplo abaixo:

```html
<html>
<head>
    <meta charset="utf8">
    <title>{{page.title}}</title>
</head>
```

Neste exemplo foi utilizado o prefixo `page` pois estamos acessando os valores da página declarados no topo utilizando front-matter **YAML**, quando for fazer referência ao site você deve utilizar o prefixo `site`, os valores utilizados a partir do prefixo `site` são obtidos do arquivo **_config.yml**.

Neste post apresentei as tecnologias envolvidas e os principios do jekyll e de como utiliza-lo. Ficou interessado no post  **[Instalando o Jekyll](https://josiasmaceda.com.br/web/jekyll/2016/06/11/instalando-o-jekyll.html "clique aqui")** eu mostro como fazer a instalação e começar a diversão.  

See you next post!!.