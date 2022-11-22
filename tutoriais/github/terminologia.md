---
layout: tutorial-github
title: Tutorial | GitHub e open source - Terminologia essencial
permalink: /tutoriais/github/terminologia/
---

**Índice de termos nesta página:**

- [Terminologia essencial](#terminologia-essencial)
  - [Repositório](#repositório)
  - [Issues (Problemas)](#issues-problemas)
  - [Working copy vs. Remote copy](#working-copy-vs-remote-copy)
  - [Master, Branch e Tag](#master-branch-e-tag)
  - [Operações do Git](#operações-do-git)
    - [Clone](#clone)
    - [Fork](#fork)
    - [Add, Stage, Commit e Push](#add-stage-commit-e-push)
    - [Pull](#pull)
    - [Pull request](#pull-request)
    - [Merge](#merge)
  - [Tracked vs. Untracked (Versionado e não versionado)](#tracked-vs-untracked-versionado-e-não-versionado)
  - [Docs-as-code](#docs-as-code)
  - [Juntando tudo: o ciclo completo](#juntando-tudo-o-ciclo-completo)

# <a name="terminologia-essencial"></a>Terminologia essencial

Este tópico apresenta uma lista de termos que são essenciais para trabalhar com o Git. Existem muito mais palavras e operações associadas a este sistema de controle de versão, mas aqui estão as mais usadas no dia a dia e que você precisa para completar o tutorial.

Lembre-se: você não precisa saber *como* executar os comandos do Git em um terminal, mas você precisa pelo menos saber *quais* existem e *o que* eles fazem. Esta documentação deve ajudar nesta parte.

---

## <a name="repositório"></a>Repositório

**Repositório** é o local onde um projeto fica armazenado no sistema de controle de versão. Dentro do repositório, ficam guardados todos os arquivos fonte do projeto.

Cada repositório pode ser configurado como **público** ou **privado**. Se o repositório estiver público, qualquer pessoa pode acessá-lo. Se for privado, somente o dono do repositório tem acesso.

Uma conta no GitHub pode ter múltiplos repositórios.

## <a name="issues-problemas"></a>Issues (Problemas)

Uma **issue** é uma espécie de "ticket" que é aberto para um projeto.

As pessoas usam issues para:

* relatar problemas no funcionamento do projeto
* pedir melhorias ou novas implementações no projeto
* controlar o andamento desses pedidos

Em projetos públicos, qualquer pessoa que tenha conta no GitHub pode abrir uma issue.

## <a name="working-copy-vs-remote-copy"></a>Working copy vs. Remote copy

O repositório que está no GitHub é chamado de **remote copy** (ou cópia remota).

É possível fazer o download da cópia remota de um projeto e trabalhar nele localmente. A cópia baixada é chamada de **working copy** (ou cópia de trabalho).

## <a name="master-branch-e-tag"></a>Master, Branch e Tag

Como foi dito no [tópico sobre Git e GitHub](/tutoriais/github/git-github/), um sistema de controle de versão permite que você trabalhe com diferentes revisões de um mesmo arquivo simultaneamente. O controle de versão permite também trabalhar com versões do seu projeto inteiro.

A versão principal do seu projeto (versão de produção) é o **master**.

Você pode criar ramificações do master, as quais podem ser alteradas de maneira independente. Cada ramificação é chamada de **branch**. Branches permitem fazer grandes alterações sem afetar a versão de produção.

**Tag** é uma maneira de identificar os grandes marcos do seu projeto. No caso de um software, tags podem representar grandes releases do produto. Tags são associados aos branches dos grandes releases, facilitando a identificação de versões específicas.

## <a name="operações-do-git"></a>Operações do Git

### <a name="clone"></a>Clone

**Clone** é a ação de baixar o projeto para um ambiente local. Ou seja, fazer o download da cópia remota do projeto para obter uma cópia de trabalho (local). Por exemplo, se você precisa baixar o projeto do TW Livre para alterá-lo, você precisa fazer um clone do projeto.

### <a name="fork"></a>Fork

**Fork** é a ação de criar uma cópia do repositório de uma conta do GitHub para a sua própria conta. Esta ação é necessária para que você contribua com projetos open source, então esta é uma ação muito importante, assim como o pull request (explicado mais adiante).

### <a name="add-stage-commit-e-push"></a>Add, Stage, Commit e Push

Depois que você faz o clone de um projeto para o seu ambiente local, você pode começar a alterar o projeto. Depois de alterar, você precisa enviar as alterações para a cópia remota.

O processo de envio de uma cópia de trabalho (local) para a cópia remota (repositório) envolve quatro operações principais: **add**, **stage**, **commit** e **push**.

Estas são as descrições de cada operação, na ordem em que elas devem ser feitas:

1. **Add :** esta operação acontece naturalmente no momento em que você cria ou altera um arquivo no projeto. Quando o Git percebe que você alterou um arquivo, ele automaticamente faz a ação de Add. Portanto, o add significa basicamente que o arquivo está marcado como alterado.
2. **Stage:** o stage consiste em pegar um arquivo marcado como alterado (add) e sinalizar que ele está numa fila para ser consolidado no projeto. Ao fazer um stage em um arquivo, você estará indicando que provavelmente não fará mais nenhuma alteração neste arquivo.
   * Dica: nesse momento, você ainda pode revisar as alterações e escolher não seguir em frente. Existe a operação de **unstage**, que volta o arquivo para a situação de add.
3. **Commit:** o commit é um estágio além do stage. O commit é o comando que indica que você realmente não tem mais nada a alterar em um arquivo. É o último estágio antes de enviar as alterações do ambiente local para o repositório.
4. **Push:** o push é a operação que envia os arquivos da cópia de trabalho (local) para a cópia remota. Esta operação pega todos os arquivos que passaram pelo commit e os envia para o seu repositório.

Estas operações são os estágios em que suas alterações precisam passar para chegar da sua cópia de trabalho até a cópia remota.

Você pode fazer uma analogia destas operações com as etapas do envio de um e-mail:

* **Add:** neste estágio, você começou a escrever um e-mail, mas ainda não terminou. Você ainda tem coisas para escrever e está trabalhando nele.
* **Stage:** aqui você acredita que escreveu tudo que tinha para escrever no e-mail e salvou ele na pasta de rascunhos, para uma última revisão.
* **Commit:** você revisou o e-mail, considerou que está tudo certo e enviou a mensagem. Aqui o e-mail foi para a caixa de saída e está pronta para ir para o destinarário.
* **Push:** você acessou a caixa de saída, enviou o e-mail e o destinatário recebeu a mensagem. O processo está completo.

### <a name="pull"></a>Pull

O **pull** é o comando que puxa as alterações do repositório (remoto) para a sua cópia de trabalho (local).

As alterações obtidas pelo pull podem ter sido feitas por você mesmo (diretamente no repositório) ou por outra pessoa que esteja contribuindo com o seu projeto.

O pull é importante para manter os projetos sincronizados. De maneira geral, recomenda-se sempre fazer um pull antes de começar a alterar algum arquivo do projeto. Esta prática garante que você está trabalhando na versão mais recente dos arquivos.

### <a name="pull-request"></a>Pull request

**Pull request** é a operação que envia uma alteração de um repositório para outro.

Ao contribuir com open source, você não fará um push diretamente para o projeto. Você primeiro precisa fazer um fork, alterar o seu fork projeto e enviar um pedido para o projeto original "incorporar" suas alterações. Este pedido de incorporação das alterações é o pull request.

Uma pessoa responsável pelo projeto original irá receber seu pull request, analisá-lo e decidir o que fazer com o pedido.

No final deste tópico está uma explicação do processo completo até chegar no pull request.

### <a name="merge"></a>Merge

Depois que você termina de trabalhar com um branch, você precisa incorporar as alterações deste branch para outro (normalmente o Master). Esta operação de incorporar um branch a outro se chama **merge**.

O merge evita que todas as alterações feitas em um branch precisem ser replicadas manualmente para outro branch. Esta operação também permite que alguém revise a junção das alterações entre os branches, antes de enviar para o Master.

## <a name="tracked-vs-untracked-versionado-e-não-versionado"></a>Tracked vs. Untracked (Versionado e não versionado)

**Tracked** e **untracked** são as situações em que um arquivo se encontra no seu working copy.

* **Untracked** é a situação de novos arquivos que você cria no working copy e que ainda não foram enviados para o repositório. Portanto, o arquivo ainda não está versionado; o arquivo ainda não está sob domínio do controle de versão.
* **Tracked** é as situação de arquivos que já foram enviados do working copy para o repositório. Ou seja, arquivos que já estão passando pelo controle de versão e têm suas alterações detectadas pelo sistema.

## <a name="docs-as-code"></a>Docs-as-code

**Docs-as-code** ("documentação como código") é o conceito de trabalhar com múltiplas revisões da documentação e versioná-la.

Para saber mais sobre este conceito, acesse o tópico sobre [controle de versão](/tutoriais/github/controle-versao/).

---

## Juntando tudo: o ciclo completo

1. Faz o **fork** do projeto TW Livre, criando assim uma cópia remota na sua própria conta do GitHub.
2. Faz o **clone** do repositório da sua conta (obtido pelo Fork), criando assim uma cópia local.
3. Altera os arquivos na sua cópia local, colocando os arquivos como **Add**.
4. Passa os arquivos alterados por todos os estágios seguintes - **Stage**, **Commit** e **Pull** -, enviando assim todas as alterações para a cópia remota na sua própria conta do GitHub.
5. Faz um **pull request** das alterações, enviando-as do repositório na sua conta para o repositório de origem.
6. A pessoa responsável pelo repositório de origem recebe o seu pull request e analisa as alterações. Aqui ela normalmente faz o seguinte:
    * Decide que suas alterações estão corretas e são válidas. Então, ela faz o **merge** das alterações, incorporando-as ao projeto de origem.
    * Decide que suas alterações precisam de ajustes e sugere alterações. Então, você faz os ajustes e envia um novo **pull request**, que volta para o ciclo de aprovação.

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/github/ferramentas/"><button type="button" class="btn btn-dark">Ferramentas</button></a></p>
