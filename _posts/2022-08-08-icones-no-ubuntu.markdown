---
layout: post
title:  "Ubuntu, atalhos"
date:   2022-08-08
---

<p class="intro"><span class="dropcap">N</span>o Ubuntu é possivel criar atalhos e icones para aplicações. Iremos ver como criar um atalho para uma aplicação no Ubuntu.</p>

O primeiro passo é ter a aplicação (caminho para executa-la) e o icone para o atalho. Vá até a pasta `~/.local/share/applications/` e crie um arquivo com o nome `meuArquivo.desktop`.

{%- highlight bash -%}

$ cd ~/.local/share/applications/

$ > meuArquivo.desktop

{%- endhighlight -%}

Nesse arquivo povoe com a seguinte estrutura:

```
[Desktop Entry]
Version=1.0
Type=Application
Name=meuApp
Comment=Comentário
Exec= ./app
Icon=CaminhoParaOicone
Path=CaminhoParaOaplicativo
Terminal=false
StartupNotify=false
```

Pronto agora podemos ter o icone e o atalho para executar a aplicação.