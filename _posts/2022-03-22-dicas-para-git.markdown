---
layout: post
title:  "GIT, dicas e lembretes"
date:   2022-03-22
---

<p class="intro"><span class="dropcap">O</span> GIT é uma versionador descentralizada de arquivos, e aqui vão algumas dicas e macetes para utilizar essa ferramenta.</p>

A ideia dessa página é servir de memorix para utilizar a ferramenta, portanto sempre que eu sentir necessidade irei atualizar com novos comandos e dicas de como podemos usar melhor a ferramenta, lembrando que é frente a minha experiência.

## Criando uma TAG

TAGs geralmente são usadas para indicar versões. São muito úteis e por costume fazemos na MAINLINE (lembrando que esse processo é feito após MERGES e a MAIN estar atualizada). Para criar uma TAG:

{%- highlight bash -%}

$ git tag -a <name> -m <message>

{%- endhighlight -%}

Com a TAG criada, basta "empurrar" para o server:

{%- highlight bash -%}

$ git push origin <TAG_name>

{%- endhighlight -%}