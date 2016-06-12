---
layout: post
title: "Instalando e configurando o Jekyll"
date: 2016-06-11 18:38:00
comments: true
disqus: true
author: josiasmaceda
categories: web jekyll
---

Primeiramente você deve baixar o Servidor de sites estáticos **[Jekyll](http://jekyllrb.com/ "Clique aqui e acesse o site do Jekyll")**


>### Instalação

Execute os comandos abaixo no shell para a instalação:

```sh	
$ gem install jekyll #Baixa e instala o servidor
$ jekyll new meublog #Cria o projeto e estrutura do blog/site
$ cd meublog #Entra na pasta do projeto
```

Para executar o servidor:

```sh
$ jekyll server -w #Lembre se de executar o comando dentro do diretório do seu projeto
```

Em seguida acesse <http://localhost:4000> e veja o servidor rodando.
O parametro `-w` faz com que o jekyll fique monitorando o projeto em busca de atualizações, e caso possua atualize os arquivos do site.

Para que o Jekyll faça o build do projeto execute o seguinte comando:

```sh
$ jekyll build
```	

O comando `Build` constroi o site com base nos arquivos e pasta de configuração.
 
	
Se você utiliza o **windows** baixe o **[Ruby Installer](http://rubyinstaller.org/downloads/ "Clique aqui para acessar a página do projeto")**.
(*lembre-se de marcar no instalador de adicionar o ruby no path do windows*). Após a instalação 
execute os mesmos comandos citados acima no powershell do windows.
	
>### Cuidados

* Se usar o nootepad++ salve ele no formato `UTF-8 without BOM`
	