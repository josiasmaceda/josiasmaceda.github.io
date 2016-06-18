---
layout: post
title: "Instalando o Jekyll"
date: 2016-06-11 18:38:00
comments: true
disqus: true
author: josiasmaceda
categories: web jekyll
---

![Jekyll](https://jekyllrb.com/img/logo-2x.png)

Welcome! Neste meu primeiro post irei apresentar como fazer para baixar e instalar o gerador de sites estáticos **[Jekyll](http://jekyllrb.com/ "Clique aqui e acesse o site do Jekyll")**


>### Instalação

Primeiramente temos que destacar que o jekyll é criado em Ruby, logo temos que ter ele instalado na máquina.  
Caso não tenha instalado o Ruby, execute o seguinte comando para instalação no Debian ou Ubuntu:

```sh
$ sudo apt-get install ruby-full
```

E caso você utilize o **windows** baixe o **[Ruby Installer](http://rubyinstaller.org/downloads/ "Clique aqui para acessar a página do projeto")**.
(*lembre-se de marcar no instalador de adicionar o ruby no path do windows*).

Para outros sistemas operacionais basta executar as instruções **[aqui](https://www.ruby-lang.org/en/documentation/installation/ "Clique aqui para instruções de instalação em outros SOs")**.

Enfim, para a instalação do Jekyll basta executar os seguintes comandos no shell:

```sh	
$ gem install jekyll #Baixa e instala o servidor
$ jekyll new meublog #Cria o projeto e estrutura do blog/site
$ cd meublog #Entra na pasta do projeto
```

Para verificar se foi instalado com sucesso execute o seguinte comando para que seja iniciado um servidor na porta 4000:

```sh
$ jekyll server -w #Lembre se de executar o comando dentro do diretório do seu projeto
```

Em seguida acesse <http://localhost:4000> e veja o servidor rodando.
O parametro `-w` faz com que o jekyll fique monitorando o projeto em busca de atualizações, e caso possua atualize os arquivos do site.

Para que o Jekyll faça o build do projeto execute o seguinte comando:

```sh
$ jekyll build
```	

O comando `Build` constroi o site com base nos arquivos e pastas de configuração do jekyll e gera o site na pasta `_site` dentro do seu projeto.
 
Done! Agora já temos nosso gerador de sites estáticos, instalado e rodando.  
See you next post...	
	
>### Cuidados

* Se usar o nootepad++ salve ele no formato `UTF-8 without BOM`
	