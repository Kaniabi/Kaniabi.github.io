---
layout: post
title:  "Introdução ao Linux"
date:   2015-11-11 22:06:00 -0200
categories: linux
---
Um pequeno check-list para ensinar/aprender sobre o linux.

Referencia: [http://www.tldp.org/LDP/intro-linux/html/](http://www.tldp.org/LDP/intro-linux/html/)

# O que é Linux?

* Linux (todas as variações) são implementações de um sistema UNIX;
 * http://i.stack.imgur.com/G2Xri.png
* No versionamento de uma distribuição linux existe a versão do CORE e a versão da distribuição;
* Implementado em C, linguagem essa que foi desenvolvida para ele;
* Existem muitos sabore de Linux, os dois principais branches são redhat e debian;
 * Muitos sabores (flavours):
  * Redhat
  * Debian
 * Ferramentas da GNU (shell, compilador)

# Contas

* Conta `root` é o administrador do sistema, mas deve-se evitar usá-la uma vez
que "com muito poder vem muitas responsabilidade".
 * Exemplo, ao tentar deletar um diretório local chamado `bin` pode-se tentar
 executar o comando `rm -rf /bin`. Como root, ele vai fazer o que você mandou.

# Check-list de conceitos

* O shell é um programa como qualquer outro que te dá acesso a navegar e alterar
  arquivos e diretórios além de chamar outros comandos;
* Como tudo no mundo Linux, existem diversos sabores, o mais comum é o `bash`;
* O sistema de arquivos do Linux tem três hierarquias:
 * Disco: elementos de armazenamento físicos;
 * Partições: armazenamento lógico. Pode-se ter uma partição com vários discos
   nela ou vice-versa;
 * Sistema de arquivos

# Sistema de Arquivos

* Arquivos são arquivos e diretórios são "organizadores recursivos de arquivos";
* Todo arquivo/diretório possui um dono e um grupo;
* Não existem drives no sistema de arquivos do Linux como existe no Windows. Todos os arquivos estão dentro do "/";
* O sistema de permissão do linux é baseado em três níveis:
 * dono (owner)
 * grupo (group)
 * todos (all)
* Para cada um dos níveis existem três níveis de permissões:
 * Leitura (r - read)
 * Escrita (w - write)
 * Execução (x - execution)
* Caminhos de arquivos são separados por barras "/"
* Existem caminhos locais ou absolutos


# Processos

* O shell pode iniciar processos em "background" usando `&` no final da chamada;
* Comando `jobs`, `kill` e `ps`;
* Comando `bg`e `fg`;
* `Ctrl+Z`

# Redireções

* Redirecionamento de entrada e saída usando `>`, `>>` e `<`;
* Pipes `|`;
* Filtros: `sort`, `uniq` e `grep`;
* Descritores de arquivo de entrada (`0`), saída (`1`) e erro (`2`);
* Redirecionamento de saída e erro: `2>&1`;
* Processos no tempo: `time`, `at` e `cron`/`crontab`;

# Editores de Texto

* `vim`?

# Instalando

* Gerenciadores de pacotes: `rpm`/`dbkg`/`yum`/`apt-get`
* `configure`/`make`
