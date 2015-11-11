---
layout: post
title:  "Ruby no Windows"
date:   2015-11-10 22:41:00 -0200
categories: ruby windows
---
Algumas considerações ao configurar o Ruby no Windows 10:

* Baixar instalador do site [http://rubyinstaller.org/downloads/](http://rubyinstaller.org/downloads/);
* Como sugerido, usar a versão 2.1.X. Imagino que o Ruby deve sofrer de
distúrbios de versões assim como o Python;
* Arrumar os paths.

Eu baixei o Ruby para poder usar o [jekyll](https://github.com/jekyll/jekyll). O
gerenciador de pacotes do Ruby é o `gem`.

```ruby
$ gem install jekyll
```

Depois disso tive que instalar algumas dependências que a minha configuração
específica do Jekylll precisava (`redcarpet` e `pygments`):

```ruby
$ gem install redcarpet pygments
```

Para tanto foi necessário instalar também o DevKit para o Ruby, também
disponível na página de downloads do Ruby. Resumidamente para completar a
instalação é necessário:

* Extrair o devkit (`d:/shared/devkit`);
* Inicializar o devkit (`ruby dk.rb init`);
* Alterar o arquivo de configuração de acordo com as versões de Ruby instaladas (`config.yml`);
* Instalar o devkit (`ruby dk.rb install`).

Um toque final, para usar o gem de dentro da [Take Command](https://jpsoft.com/take-command-windows-scripting.html) foi necessário
chamar ele via `cmd`.

```console
$ cmd /c gem install redcarpet
```
