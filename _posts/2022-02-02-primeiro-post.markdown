---
layout: post
title:  "Meu Primeiro Post"
date:   2022-02-02
---

<p class="intro"><span class="dropcap">N</span>este primeiro post irei explicar como criar seu blog utilizando Jekyll e o Gitub.</p>

Jekyll é um Framework (gerador de sites estaticos) desenvolvido em [Ruby][ruby_docs], pratico e fácil de usar. Atravez do Github podemos ter um blog em poucos passos.

Instalação de ferramentas necessárias:
{%- highlight shell -%}
$ sudo apt install git

$ sudo apt install ruby-full build-essential zlib1g-dev rubygems 
{%- endhighlight -%}

Para instalar o Jekyll basta rodar o seguinte comando:
{%- highlight shell -%}
$ gem install jekyll bundler
{%- endhighlight -%}

O proximo passo é editar o arquivo gemfile, lá é explicado a dinamica da ferramenta. No meu caso:
{%- highlight shell -%}
# Comentar a linha:
gem "jekyll", "~> 4.2.1"

# E descomentar a linha
gem "github-pages", group: :jekyll_plugins
{%- endhighlight -%}

Após basta rodar o comando:
{%- highlight shell -%}
$ bundle update github-pages
{%- endhighlight -%}

Aqui tive a seguinte saida:
{%- highlight shell -%}
Bundler could not find compatible versions for gem "jekyll-feed":
  In snapshot (Gemfile.lock):
    jekyll-feed (>= 0.16.0)

  In Gemfile:
    github-pages was resolved to 36, which depends on
      jekyll-feed (= 0.2.3)

    minima (~> 2.5) was resolved to 2.5.1, which depends on
      jekyll-feed (~> 0.9)

Running `bundle update` will rebuild your snapshot from scratch, using only
the gems in your Gemfile, which may resolve the conflict.
{%- endhighlight -%}

Como podemos ver, não existe uma versão "candidata", ou melhor, compativel para o jekyll-feed, para resolver isso executei o comando:
{%- highlight shell -%}
$ bundle update jekyll-feed
{%- endhighlight -%}

Pronto, agora já temos um blog "funcional". 
O proximo passo é postar esse site no Github, para isso devemos criar um repositório com (esse passo é importante) o mesmo nome do seu usuário do Github seguidos de "github.io". Como exemplo:
{%- highlight shell -%}
[SEU_USER].github.io
{%- endhighlight -%}

Agora basta fazer um "push" do Jekyll que criamos, para o github no repositório recem criado.

Veja a documentação do [Jekyll docs][jekyll] e do [Github][github_docs] para mais informações.

[github_docs]: https://pages.github.com
[jekyll]:      http://jekyllrb.com
[ruby_docs]:   https://www.ruby-lang.org/pt/documentation/installation/