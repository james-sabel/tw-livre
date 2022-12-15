---
layout: tutorial-github
title: Tutorial | GitHub e open source - Controle de versão (Parte 1)
permalink: /tutoriais/github/controle-versao/
---

# Controle de versão

Este tópico tem os conceitos que você precisa saber sobre **controle de versão** para começar a contribuir com suas docs.

## O que é controle de versão

Controle de versão é um **sistema** que possibilita trabalhar com diferentes instâncias de um mesmo documento. Você pode encarar o controle de versão como uma forma de manter o histórico de alterações no documento, mas envolvendo operações mais complexas e avançadas.

Pessoas que trabalham com sistemas de versão criam e alteram documentos existentes no seu **ambiente local**. Depois, enviam os documentos para o sistema de controle de versão, onde ficam armazenados no **ambiente remoto**. O ambiente remoto é chamado de **repositório**.

## O que faz um sistema de controle de versão

* possibilita que múltiplas pessoas contribuam em um mesmo projeto ao mesmo tempo
* mantém um histórico de tudo que foi alterado no projeto, desde a criação
* possibilita trabalhar paralelamente em diferentes versões de um mesmo projeto e juntá-las ao longo do caminho
* controla a publicação do conteúdo conforme as releases de um projeto

## Quais sistemas de controle de versão existem

Uma lista resumida de sistemas de controle de versão pode ser consultada na [Wikipedia](https://pt.wikipedia.org/wiki/Categoria:Sistemas_de_controlo_de_vers%C3%A3o). Porém, existem muito mais sistemas além dos que estão listados no artigo.

Este tutorial adotou o **[Git](https://git-scm.com/)** como sistema de controle de versão. Este sistema é um dos mais comuns e é o sistema usado pelo **GitHub**. Você irá saber mais sobre isto no próximo tópico: [O que são Git e GitHub](/tutoriais/github/git-github/).

## Docs-as-code: documentação versionada

Assim como ocorre com um código de software colaborativo, você ou uma equipe podem manter diferentes versões da documentação do projeto. Cada nova versão gerada é chamada de **revisão**.

O conceito de revisões é aplicado ao código-fonte dos projetos, mas também pode ser aplicado para a documentação. Por isso, surge o termo **docs-as-code** (ou "documentação como código").

A prática de docs-as-code indica que a documentação é tratada da mesma maneira que o código-fonte: a documentação **está no repositório** do projeto, é **versionada** e **segue o mesmo fluxo** de trabalho, onde as pessoas colaboram com alterações.

## Como funciona um sistema de controle de versão

### Princípios básicos

* Quando uma pessoa cria ou altera documentos no **ambiente local**, depois ela precisa enviar as alterações para o **ambiente remoto** (**repositório**).
* Cada vez que um documento é enviado para o repositório, o documento ganha uma nova **revisão**. Ou seja, um mesmo documento terá diversas revisões. As revisões serão incrementadas cada vez que o documento for alterado no repositório.
* Documentos que estão no repositório podem ser acessados por qualquer membro do time.

### Cenário de exemplo

Vamos criar um cenário de exemplo para entender melhor como funciona o controle de versão.

Imagine que você tem dois tech writers no time: o **Tech Writer A** (**TW A**) e o **Tech Writer B** (**TW B**). Ambos estão trabalhando no mesmo repositório de documentação. O repositório é novo e ainda não tem nenhum documento armazenado.

Acompanhe esta sequência de ações:

#### Cada TW criou a primeira versão de um documento e enviou para o repositório

<img src="/res/img/github/version-control-1.png" alt="Imagem representando o cenário até aqui." title="TW A e B criando os documentos A e B e enviando para o repositório." style="margin-top: 15px; margin-bottom: 15px;" />

Nesse momento, os arquivos que os **TW A** e **B** criaram estão no repositório. Esta é a versão inicial dos documentos, portanto, ambos estão na **primeira revisão** (**V1**), tanto no repositório quanto nos ambientes locais onde foram criados.

<img src="/res/img/github/version-control-2.png" alt="Imagem representando o cenário até aqui." title="Os documentos A e B estão na primeira revisão, tanto no repositório quanto nos ambientes locais onde foram criados." style="margin-top: 15px; margin-bottom: 15px;" />

Imagine que o **TW A** precisa fazer alterações no **DOC B**, que foi criado por outra pessoa do time:

#### O **TW A** puxou o **DOC B** do repositório

<img src="/res/img/github/version-control-3.png" alt="Imagem representando o cenário até aqui." title="TW A puxando o DOC B do repositório." style="margin-top: 15px; margin-bottom: 15px;" />

#### O **TW A** fez as alterações no **DOC B**, gerando a **segunda revisão** (**V2**) do documento

#### O **TW A** enviou a **V2** do **DOC B** de volta para o repositório

<img src="/res/img/github/version-control-4.png" alt="Imagem representando o cenário até aqui." title="TW A alterando o DOC B e enviando de volta para o repositório." style="margin-top: 15px; margin-bottom: 15px;" />

Neste ponto, a versão do **DOC B** que está no ambiente local do **TW B** está desatualizada, pois ainda está na primeira revisão.

Para continuar mexendo no **DOC B**, o **TW B** precisaria primeiro puxar a nova revisão do repositório. Depois, trabalharia normalmente no documento.

### Mais complexidade: conflitos

O exemplo anterior mostra que o conceito de controle de versão é simples. Mas, quanto maior o volume e mais extensos forem os documentos, maior é a complexidade do controle de versão. A complexidade aumenta também com a quantidade de pessoas trabalhando juntas nos arquivos de um mesmo projeto.

Em alguns casos, pode acontecer de duas pessoas mexerem no mesmo arquivo sem que tenham puxado a versão mais recente primeiro. Quando isso acontece, ocorre um **conflito**. Conflito é o nome que se dá para a situação em que o sistema de controle de versão encontra divergências entre as revisões de um mesmo documento. Quando acontece um conflito, você precisa dizer ao sistema o que ele deve fazer com o arquivo conflitante.

Existem três opções principais do que fazer com um conflito:

* descartar suas próprias alterações e ficar com a revisão encontrada
* descartar as alterações da revisão encontrada e ficar com a sua
* juntar as alterações das duas revisões

O conflito é um cenário atípico e não será abordado neste tutorial. É interessante conhecer pelo menos os princípios básicos, pois fazem parte do cotidiano de trabalhar com controle de versão.

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/github/git-github//"><button type="button" class="btn btn-dark">O que são Git e GitHub</button></a></p>
