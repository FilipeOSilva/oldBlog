---
layout: post
title:  "Postman, dicas e lembretes"
date:   2022-05-30
---

<p class="intro"><span class="dropcap">O</span> POSTMAN é uma ferramenta utilizada para validar APIs e aqui vão algumas dicas e macetes para melhor utiliza-lo.</p>

A ideia dessa página é servir de memorix para utilizar a ferramenta, portanto sempre que eu sentir necessidade irei atualizar com novos comandos e dicas de como podemos usa-la melhor, lembrando que é frente a minha experiência.

## Criando uma Collection 

Collection, são uma maneira de organizar melhor suas requisições, possibilitando que você as exporte (para enviar para alguem) ou importe (quando recebe de alguem).
As figuras a seguir servem para demonstrar como fazer isso:

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_01.jpg" alt=""> 

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_02.jpg" alt=""> 

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_03.jpg" alt=""> 

Com a Collection criada, basta ir salvando as requisções dentro dela. Para isso em uma requisição basta clicar em "Salva como..." indiciar a coleção e salvar.

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_04.jpg" alt=""> 

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_05.jpg" alt=""> 

## Criando um Environments

Environments, são as variaveis de ambiente. Podemos manipular variaveis desde do indereço da URL até retornos das repostas das requições (via Test). Para criar um Environment, basta clicar no botão "Manage Environment". 

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_06.jpg" alt=""> 

Na tela MANAGE ENVIRONMENTS, clique em Add. 

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_07.jpg" alt=""> 

De um nome para o Environment, e pronto podemos criar as variaveis. Após isso selecione o Environment que será usado.

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_08.jpg" alt=""> 

## Criando um Test

Os Tests nos possibilitam criar automações e/ou validações das requisições. Para isso vá até o campo tests e podemos começar a edição (em javascript) dos retornos.

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_09.jpg" alt=""> 

Exemplo de como extrair um campo da resposta (em jSON).

<img src="/assets/img/2022-05-30-dicas-postman/new_collection_postman_10.jpg" alt=""> 






