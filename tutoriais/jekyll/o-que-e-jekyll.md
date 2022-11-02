---
layout: tutorial-jekyll
title: Tutorial | Jekyll - O que é
permalink: /tutoriais/jekyll/o-que-e-jekyll/
---

# O que é Jekyll

O **Jekyll é um gerador de sites estáticos**. Um site estático é livre de elementos dinâmicos.

Um site é considerado estático quando não há alterações no conteúdo durante a comunicação no [modelo cliente-servidor](https://pt.wikipedia.org/wiki/Modelo_cliente%E2%80%93servidor). Entre os benefícios deste tipo de site estão a segurança, a velocidade e a estabilidade.

Por causa da simplicidade e eficiência do resultado obtido com o Jekyll, ele é bastante usado para criar e gerar documentação.

## Que tipos de sites o Jekyll pode gerar

O Jekyll é usado para **gerar sites estáticos**, misturando **texto**, **código** e **desenvolvimento web**. Ele é muito usado para gerar blogs, com uma infinidade de recursos e customizações, mas também faz um ótimo trabalho para edição e publicação de documentação de software.

O site e as páginas são geradas a partir de arquivos-fonte em diversos formatos. Inclusive, um dos recursos mais úteis do Jekyll é unir diferentes linguagens web com linguagens usadas na documentação de software, como o **Markdown**.

## Principais componentes do Jekyll

Estes são os principais componentes e características do Jekyll:

### Ruby e Gems

O Jekyll foi desenvolvido usando a linguagem de programação **Ruby**. Por ter sido construído nesta linguagem, o Jekyll precisa que o ambiente do Ruby esteja instalado na máquina onde ele será executado.

O Ruby permite usar pacotes, que são chamados de **Gems**. O Jekyll é um dos Gems que podem ser instalados no Ruby. Portanto, existe essa dependência.

### Bundler

**Bundler** também é um **Gem** suportado pelo Ruby.

O Bundler é usado pelo Jekyll para compilar os arquivos que você vai criar, seja em Markdown, HTML, CSS ou qualquer outro formato que você escolher para construir o conteúdo.

Esse processo de compilação é chamado de **build**, que é responsável por juntar todos os seus arquivos e **gerar um output**.

O **output** é a saída final do seu site estático, que é gerado a partir dos arquivos-fonte e pronto para ser visualizado.

### Command based

O Jekyll é uma ferramenta **command based**. Isto significa que ele é operado por meio de comandos executados em um terminal, como o **prompt de comando do Windows** ou o **Bash**.

Ao longo do tutorial você vai conhecer os comandos necessários para executar as operações básicas do Jekyll. As operações citadas no tutorial são necessárias para manipular e gerar o seu projeto.

Para executar os comandos do Jekyll, você precisa estar confortável em lidar com ambientes command based.

## Formatos suportados

Estes são alguns dos formatos e linguagens suportados pelo Jekyll:

### Markdown (.MD)

O **Markdown** é uma das linguagens mais comuns para criar e gerar documentação. O Markdown é quase universal e integra bem com ambientes como o [GitHub](https://github.com/). Então, não é por acaso que o Jekyll tem total suporte para este formato de conteúdo.

O Markdown tem sintaxe própria, a qual determina como o texto será interpretado e apresentado no output. Por exemplo, se você quiser escrever um título de uma página usando Markdown, você deve escrever: `# Isto é um título`. O sustenido (#) antes da frase faz com que esta linha seja interpretada como um título.

Se você está acostumado com HTML e criação de conteúdo para a web, as coisas ficam mais simples ao saber que isso será interpretado como um `<h1>`. O mesmo acontece para diversos outros elementos em HTML, permitindo criar outros níveis de heading, links, inserir imagens, estilizar o texto e muito mais.

Uma breve pesquisa por "markdown cheatsheet" no Google deve trazer vários resultados de como escrever usando a notação em Markdown. Uma boa referência é a [página de Markdown do GitHub](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

Os arquivos escritos em Markdown podem ser salvos com as extensões **.markdown** ou **.md** — ambas funcionam do mesmo jeito.

#### Tipos alternativos de Markdown

É importante saber que hoje em dia existem versões distintas de Markdown.

Existe a versão pura — chamada "plain" ou "vanilla" — que é a versão mais básica do Markdown. Esta versão é interpretada por praticamente todas as ferramentas que suportam Markdown. Portanto, esta é a versão mais segura e prática com a qual você pode trabalhar.

Mas existem também versões alternativas que são interpretadas apenas por plataformas e ferramentas específicas. Estas versões foram criadas para:

* ampliar o leque de possibilidades oferecidas pelo Markdown puro
* aumentar o número de customizações possíveis
* simplificar a sintaxe do Markdown puro

Se você nunca mexeu com Markdown antes, este tutorial recomenda começar a particar a versão pura primeiro. Depois, avalie as ferramentas que você usará no dia a dia para determinar quais variações valem a pena você conhecer.

### Liquid

Outra linguagem usada pelo Jekyll é o **Liquid**.

Se você não é developer ou não conhece lógica de programação, o Liquid pode ser uma notação um pouco mais complexa de se entender.

O Liquid não é obrigatório para usar o Jekyll, mas é preciso estudá-lo para aproveitar o máximo das possibilidades do Jekyll. O Liquid permite que você crie recursos para ganhar tempo, melhorar a estrutura do seu projeto de documentação e usar outros recursos avançados.

Este guia usa somente alguns dos recursos disponíveis do Liquid, tais como o {% raw %}`{{ content }}` e o `{% include %}`{% endraw %}. Mas não se preocupe com isso agora — você aprenderá a usá-los ao longo do tutorial.

Se você quiser se aprofundar nos outros recursos do Liquid, você pode consultar a [documentação oficial](https://shopify.github.io/liquid/).

## Softwares de edição recomendados

Para facilitar a criação da documentação usando Markdown e Liquid, é importante usar um bom software que permita editar **texto e código** (*text+code*).

Você também pode usar um processador de texto qualquer e salvá-lo no formato **.md**, por exemplo. Desde que o texto esteja com a sintaxe e formato corretos, vai funcionar. Mas a criação de um site usando o Jekyll permite misturar diversas linguagens.

Usando um editor text+code, você vai criar conteúdo muito mais facilmente, pois este tipo de editor facilita o controle dos seus arquivos e das linguagens que você vai usar.

Um bom editor de código é o [Visual Studio Code (VSCode)](https://code.visualstudio.com/), por ser bem completo e integrar bem com ambientes de desenvolvimento. O VSCode costuma ter mais funcionalidades e plugins disponíveis.

Outra alternativa é o [Sublime Text](https://www.sublimetext.com/), que é mais básico e fácil para quem nunca mexeu com esse tipo de software antes. O Sublime Text é mais limpo e intuitivo e também é o software usado como exemplo ao longo deste tutorial.

Tanto o VSCode quanto o Sublime Text são gratuitos e facilitam o rabalho com diversos formatos ao mesmo tempo. Ambos os softwares também têm bastante suporte das comunidades e permitem instalar extensões que trazem ainda mais recursos.

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/jekyll/instalacao/"><button type="button" class="btn btn-dark">Instalação</button></a></p>
