---
layout: tutorial-github
title: Tutorial | GitHub e open source - Git e GitHub
permalink: /tutoriais/github/git-github/
---

# O que são Git e GitHub

Este tópico apresenta um conceito básico e uma breve introdução sobre Git e GitHub. Estes são os conceitos que você precisa para o tutorial do TW Livre.

Note que [o GitHub tem a sua própria documentação](https://docs.github.com/pt) com informações mais detalhadas, caso você queira se aprofundar. (Alguns trechos da documentação oficial do GitHub não está disponível em português.)

## Git

Para entender o Git, primeiro é preciso entender o que é um **sistema de controle de versão**. Se você não está familiarizado, acesse o [tópico sobre controle de versão para saber mais sobre o tema](/tutoriais/github/controle-versao/).

O Git é um dos vários [sistemas de controle de versão que existem](https://pt.wikipedia.org/wiki/Categoria:Sistemas_de_controlo_de_vers%C3%A3o). Ele é também o sistema usado pelo GitHub e , por isso, é o sistema que aparece neste tutorial.

O Git é *command based*. Isto significa que, para cada operação que você precisa fazer, você precisa executar uma linha de comando em um terminal.

## GitHub

O GitHub é uma plataforma que hospeda **arquivos de código-fonte** e permite o **controle de versão** destes arquivos por meio do **Git**. Existem outras plataformas deste tipo, mas o GitHub é uma das mais usadas e conhecidas.

Os arquivos hospedados no GitHub ficam armazenados em **repositórios**, os quais podem ser **abertos** ou **privados**.

### Repositórios no GitHub

Esta seção explica um pouco mais sobre os repositórios do GitHub.

#### Estrutura

Conheça alguns dos principais componentes da estrutura de um repositório no GitHub:

<img src="/res/img/github/estrutura-repositorio.png" alt="Screenshot do repositório do TW Livre" title="Screenshot do repositório do TW Livre" style="height: auto; max-width: 100%;" />

1. **Identificação do repositório:** a identificação do repositório mostra:
  * o nome da conta à qual o repositório pertence
  * o nome do repositório
  * a visibilidade do repositório (se ele é público ou privado)
2. **Acompanhamento do repositório:**
  * **Pin** ou **Unpin**: colocar ou remover o repositório em uma posição de destaque no seu perfil do GitHub. Se o repositório não é seu, este botão não aparece.
  * **Watch** ou **Unwatch**: acompanhar ou parar de acompanhar as alterações feitas no repositório.
  * **Fork**: faz uma cópia do repositório para a sua conta. Saiba mais sobre esta e outras operações acessando a [próxima seção (Terminologia essencial)](/tutoriais/github/terminologia/).
  * **Star** ou **Unstar**: adicionar ou remover o repositório da sua lista de projetos favoritos no GitHub.
3. **Barra de gestão do projeto:** dispõe as principais ferramentas para gerenciar um repositório e participar dos espaços de discussão sobre ele. Você conhecerá algumas ações importantes desta parte no [tópico sobre terminologia essencial)](/tutoriais/github/terminologia/), tais como **Issues** e **Pull requests**.
4. **Versões:** permite alternar entre os **Branches** e os **Tags** do projeto. Estas definições serão melhor exploradas no [tópico sobre terminologia essencial)](/tutoriais/github/terminologia/).
5. **Ações de arquivos:** você pode pesquisar no conteúdo dos arquivos (**Go To File**), adicionar arquivos ao projeto (**Add File**) ou **clonar** o projeto.
6. **Sobre:** barra lateral com um resumo das principais informações sobre o projeto.
7. **Arquivos do repositório:** lista navegável de todos os arquivos contidos no projeto.

#### Documentação inicial do projeto

A maioria dos projetos do GitHub começa com uma documentação básica. São informações quase essenciais que apresentam o projeto e ajudam a orientar pessoas que querem contribuir.

Estes são alguns dos arquivos de docs mais comuns em projetos open-source:

* **README.md**: documentação de introdução do projeto. Descreve o que é o projeto, para que serve, a quem se destina e quais problemas ele resolve. Costuma ter links para as outras documentações do projeto.
* **CONTRIBUTION.md**: documentação de contribuição do projeto. Descreve as diretrizes, regras e orientações gerais do que precisa ser feito para contribuir. É um *guideline* que ajuda as pessoas que estão contribuindo pela primeira vez com o projeto. Note que nem todo projeto open-source aceita contribuições do público em geral. Uma documentação de contribuição normalmente ajuda a esclarecer esta e outras questões.

### Preciso saber os comandos do Git para usar o GitHub?

Você não precisa saber *como* executar os comandos do Git em um terminal, mas você precisa pelo menos saber *quais* existem e *o que* eles fazem.

Os conceitos do Git são importantes para entender o que está acontecendo nas operações com o GitHub. Estes conceitos serão abordados no próximo tópico: [terminologia essencial](/tutoriais/github/terminologia/).

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/github/terminologia/"><button type="button" class="btn btn-dark">Terminologia essencial</button></a></p>
