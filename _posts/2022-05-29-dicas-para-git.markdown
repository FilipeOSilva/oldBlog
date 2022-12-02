---
layout: post
title:  "GIT, dicas e lembretes"
date:   2022-05-29
---

<p class="intro"><span class="dropcap">O</span> GIT é uma versionador descentralizado de arquivos, e aqui vão algumas dicas e macetes para utilizar essa ferramenta.</p>

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

## Commit "supervisionado"

Existem varias maneiras de fazer um commit, mas a que mais tem me agradado é uma que possibilita revisar, alteração por alteração, em arquivo por arquivo e  ir aplicando se desejo ou não "jogar" naquele alteração neste commit. Para isso:

{%- highlight bash -%}

$ git commit -p

{%- endhighlight -%}

Com isso irá aparecer as alterações e um pequeno Menu de possibilidades:

{%- highlight bash -%}

(1/2) Stage this hunk [y,n,q,a,d,j,J,g,/,e,?]? ?
y - stage this hunk
n - do not stage this hunk
q - quit; do not stage this hunk or any of the remaining ones
a - stage this hunk and all later hunks in the file
d - do not stage this hunk or any of the later hunks in the file
g - select a hunk to go to
/ - search for a hunk matching the given regex
j - leave this hunk undecided, see next undecided hunk
J - leave this hunk undecided, see next hunk
e - manually edit the current hunk
? - print help
@@ -1,7 +1,7 @@
 ---
 layout: post
 title:  "GIT, dicas e lembretes"
-date:   2022-03-22
+date:   2022-05-29
 ---
(1/2) Stage this hunk [y,n,q,a,d,j,J,g,/,e,?]? 

{%- endhighlight -%}

Após selecionar os arquivos e alterações que serão commitadas, irá abrir o editor de texto padrão do seu terminal para que seja escrita a mensagem do commit. Salvado e saindo o commit estará feito.


