---
layout: post
title:  "SCP transitando arquivos entre servidores Linux"
date:   2022-03-15
---

<p class="intro"><span class="dropcap">O</span> scp é uma maneira rápida e pratica para transferir arquivos entre servidores Linux pelo terminal.</p>

Para utilizar o scp temos que ter o login e senha, e esse user tem que ter permissão, a máquina de onde iremos pegar e/ou enviar os arquivos.

## Enviando Arquivo

Para enviar um arquivo da sua máquina para a destinataria basta saber o endereço, ter o login e senha. Um detalhe importante é definir onde o arquivo ficará no destino:

{%- highlight bash -%}

$ scp aquivo_enviado.txt [login]@[ip_destinatario]:[/home/pasta_destino/]

{%- endhighlight -%}

## Pegando Arquivo

Para pegar um arquivo de uma máquina temos que saber o endereço, ter o login e senha. Devemos definir aonde queremos o arquivo na nossa máquina:

{%- highlight bash -%}

$ scp [login]@[ip_destinatario]:[/home/pasta_do_arquivo/arquivo_recebido.txt] .

{%- endhighlight -%}

OBS.: Aqui iremos recerber no arquivo na pasta onde estamos.

