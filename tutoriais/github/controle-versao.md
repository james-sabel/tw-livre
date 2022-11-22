---
layout: tutorial-github
title: Tutorial | GitHub e open source - Controle de versão
permalink: /tutoriais/github/controle-versao/
---

# Controle de versão

Este tópico tem os conceitos que você precisa saber sobre **controle de versão** para começar a contribuir com suas docs.

## O que é controle de versão

Controle de versão é um **sistema** que permite trabalhar com diferentes instâncias de um mesmo documento. Você pode encarar o controle de versão como uma forma de manter o histórico de alterações no documento, mas envolvendo operações mais complexas e avançadas.

Pessoas que trabalham com sistemas de versão criam documentos ou alteram documentos existentes no seu ambiente local e depois os enviam para o sistema. Ao enviar os documentos para o sistema de controle de versão, os documentos ficam armazenados no ambiente remoto. O ambiente remoto é chamado de **repositório**.

## O que faz um sistema de controle de versão

* permite múltiplas pessoas trabalharem em um mesmo projeto ao mesmo tempo
* mantém um histórico de tudo que foi alterado no projeto
* permite trabalhar paralelamente em diferentes versões de um mesmo projeto e juntá-las ao longo do caminho

## Por que usar um sistema de controle de versão

Sistemas de controle de versão têm benefícios porque permitem:

* acessar ao histórico do documento nos seus vários estágios, desde a criação
* facilitar o trabalho de equipes que trabalham nos documentos de um mesmo projeto
* controlar a publicação do conteúdo conforme as releases de um projeto

Existem outros ganhos, mas estes são os principais.

## Quais sistemas de controle de versão existem

Uma lista resumida de sistemas de controle de versão pode ser consultada na [Wikipedia](https://pt.wikipedia.org/wiki/Categoria:Sistemas_de_controlo_de_vers%C3%A3o). Porém, existem muito mais sistemas além dos que estão listados no artigo.

Este tutorial adotou o **[Git](https://git-scm.com/)** como sistema de controle de versão. Este sistema é um dos mais comuns e é o sistema usado pelo **GitHub**. Você irá saber mais sobre isto no próximo tópico: [O que são Git e GitHub](/tutoriais/github/git-github/).

## Docs-as-code: documentação versionada

Assim como ocorre com um código de software colaborativo, você ou uma equipe podem fazer operações para manter diferentes versões da documentação do projeto. Cada nova versão gerada é chamada de **revisão**.

O conceito de revisões é aplicado ao código-fonte dos projetos, mas também pode ser aplicado para a documentação. Por isso, surge o termo **docs-as-code** (ou "documentação como código").

A prática de docs-as-code indica que a documentação é tratada da mesma maneira que o código-fonte: a documentação **está no repositório** do projeto, é **versionada** e **segue o mesmo fluxo** de trabalho, onde as pessoas colaboram com alterações. Até o final deste tutorial, você terá aplicado estes conceitos na prática.

## Como funciona um sistema de controle de versão

Este tópico procura explicar os princípios básicos de controle de versão, usando cenários de exemplo com documentação.

### Princípios básicos

* Quando uma pessoa cria ou altera documentos no **ambiente local**, posteriormente ela envia as alterações para o **repositório**.
* Cada vez que um documento é enviado para o repositório, o documento ganha uma nova **revisão**. Ou seja, um mesmo documento terá diversas revisões, as quais serão incrementadas cada vez que o documento for alterado no repositório.
* Documentos que estão no repositório podem ser acessados por qualquer membro do time.

Veja o esquema abaixo:

> Imagine que você tem dois tech writers no time: **Tech Writer A** (**TWA**) e **Tech Writer B** (**TWB**). Ambos estão trabalhando no mesmo projeto de documentação e fizeram o seguinte:
>
> 1. O TWA criou o documento 1 (**Doc-1**) e enviou para o repositório.
> 2. O TWB criou o documento 2 (**Doc-2**) e enviou para o repositório.
>
> Neste ponto, ambos os documentos - Doc-1 e Doc-2 - estão na **primeira revisão** (**rev-1**).
>
> Então, ocorre o seguinte:
>
> * O TWA alterou o **Doc-2** e enviou para o repositório, gerando a **rev-2** deste documento.
>
> Neste ponto, a versão que está no ambiente local do TWB está desatualizada, pois ainda está na **rev-1**.
> Então, o TWB precisará **buscar as alterações do documento no repositório**. Com isso, o TWB atualizará o documento no seu ambiente local para a revisão mais atual - neste caso, a **rev-2**.

O exemplo acima faz parecer que controle de versão é algo bem simples. O conceito é simples, realmente. Mas, quanto maior o volume e mais extensos forem os documentos, maior é a complexidade do controle de versão. A complexidade aumenta também com a quantidade de pessoas trabalhando juntas nos arquivos de um mesmo projeto.

### Mais complexidade: conflitos

**Conflito** é o nome que se dá para a situação em que o sistema de controle de versão encontra divergências entre as revisões de um mesmo documento. Quando acontece um conflito, você precisa dizer ao sistema o que ele deve fazer com o arquivo conflitante.

Existem três opções principais do que fazer com um conflito:

* descartar suas próprias alterações e ficar com a revisão encontrada
* descartar as alterações da revisão encontrada e ficar com a sua
* juntar as alterações das duas revisões

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/github/git-github//"><button type="button" class="btn btn-dark">O que são Git e GitHub</button></a></p>
