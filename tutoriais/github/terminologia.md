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

# <a name="terminologia-essencial"></a>Terminologia essencial

Este tópico apresenta uma lista de termos essenciais para trabalhar com o Git. Existem muito mais palavras e operações associadas a este sistema de controle de versão, mas aqui estão as mais usadas no dia a dia e que você precisa para completar o tutorial.

Lembre-se: como Tech Writer, você não precisa necessariamente saber *como* executar os comandos do Git em um terminal, mas você precisa pelo menos saber *quais* existem e *o que* eles fazem. Esta documentação deve ajudar nesta parte.

---

## <a name="repositório"></a>Repositório

**Repositório** é o local onde um projeto fica armazenado no sistema de controle de versão. Dentro do repositório, ficam guardados todos os arquivos fonte do projeto.

Cada repositório pode ser configurado como **público** ou **privado**. Se o repositório estiver público, qualquer pessoa pode acessá-lo. Se for privado, somente o dono do repositório tem acesso.

Uma mesma conta no GitHub pode ter múltiplos repositórios.

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

No Git, a operação de copiar o projeto do ambiente remoto para o local se chama [**clone**](#clone).

## <a name="master-branch-e-tag"></a>Master, Branch e Tag

Como foi dito no [tópico sobre Git e GitHub](/tutoriais/github/git-github/), um sistema de controle de versão permite que você trabalhe com diferentes revisões de um mesmo arquivo simultaneamente. O controle de versão permite também trabalhar com versões do projeto inteiro.

A versão principal do seu projeto (versão de produção) é chamada **master**.

Você pode criar ramificações do master, as quais podem ser alteradas de maneira independente. Cada ramificação é chamada de **branch**. Branches permitem fazer grandes alterações sem afetar a versão de produção.

**Tag** é uma maneira de identificar os grandes marcos do seu projeto. No caso de um software, tags podem representar grandes releases do produto. Tags são associados aos branches dos grandes releases, facilitando a identificação de versões específicas.

## <a name="operações-do-git"></a>Operações do Git

### <a name="clone"></a>Clone

**Clone** é a ação de baixar o projeto para um ambiente local. Ou seja, fazer o download da cópia remota do projeto para obter uma cópia de trabalho (local). Por exemplo, se você precisa baixar o projeto do TW Livre para alterá-lo, você precisa fazer um clone do projeto.

### <a name="fork"></a>Fork

**Fork** é a ação de criar uma cópia do repositório de uma conta do GitHub para a sua própria conta.

Por exemplo, você pode fazer uma cópia do projeto do TW Livre da conta original para a sua conta pessoal no GitHub — para isso, basta fazer um fork do projeto original.

### <a name="add-stage-commit-e-push"></a>Add, Stage, Commit e Push

Quando você faz o [clone](#clone) de um projeto, você pode começar a alterá-lo no ambiente local. Depois de alterar o projeto, você precisa enviar as alterações para a cópia remota.

O processo de envio das alterações da cópia de trabalho (local) para a cópia remota (repositório) envolve quatro operações principais: **add**, **stage**, **commit** e **push**.

Estas são as descrições de cada operação, na ordem em que elas devem ser feitas:

1. **Add :** esta operação acontece naturalmente no momento em que você cria ou altera um arquivo no projeto. Quando o Git percebe que você alterou um arquivo, ele automaticamente faz a ação de Add. Portanto, o add significa basicamente que o arquivo está marcado como alterado.
2. **Stage:** o stage consiste em pegar um arquivo marcado como alterado (add) e sinalizar que ele está numa fila para ser consolidado no projeto. Ao fazer um stage em um arquivo, você estará indicando que (provavelmente) não fará mais nenhuma alteração neste arquivo.
   * Dica: nesse momento, você ainda pode revisar as alterações e escolher não seguir em frente. Existe a operação de **unstage**, que volta o arquivo para a situação de add.
3. **Commit:** o commit é um estágio além do stage. O commit é o comando que indica que você realmente não tem mais nada a alterar em um arquivo. É o último estágio antes de enviar as alterações do ambiente local para o repositório.
4. **Push:** o push é a operação que envia os arquivos da cópia de trabalho (local) para a cópia remota. Esta operação pega todos os arquivos que passaram pelo commit e os envia para o seu repositório.

<p style="text-align: center"><img src="/res/img/github/add-stage-commit-push.png" alt="Imagem representativa dos estágios de uma alteração básica no Git." title="Estágios de uma alteração básica no Git." style="margin-top: 15px; margin-bottom: 15px;" /></p>

Estas operações são os estágios em que suas alterações precisam passar para chegar da sua cópia de trabalho até a cópia remota.

Somente as pessoas que têm acesso direto ao projeto original podem fazer um push. Pessoas de fora do projeto que queiram enviar alterações, precisam fazer um [pull request](#pull-request).

### <a name="pull"></a>Pull

O **pull** é o comando que puxa as alterações do repositório (remoto) para a sua cópia de trabalho (local).

<p style="text-align: center"><img src="/res/img/github/pull.png" alt="Imagem representativa de um pull no Git." title="Pessoa fazendo o pull das alterações de um projeto no Git." style="margin-top: 15px; margin-bottom: 15px;" /></p>

As alterações obtidas pelo pull podem ter sido feitas por você mesmo (diretamente no repositório) ou por outra pessoa que esteja contribuindo com o seu projeto.

O pull é importante para manter os projetos sincronizados. De maneira geral, recomenda-se sempre fazer um pull antes de começar a alterar algum arquivo do projeto. Esta prática garante que você está trabalhando na versão mais recente dos arquivos.

### <a name="pull-request"></a>Pull request

**Pull request** é a operação que envia uma alteração de um repositório para outro.

Ao contribuir com open source, você *não* fará um push diretamente para o projeto original. Para enviar sua contribuição, você precisa:

1. Fazer um fork do projeto original.
2. Fazer um *push* das alterações para o seu projeto (criado pelo fork do passo anterior).
3. Enviar um pedido para "incorporar" as alterações do fork para o projeto original. Este pedido de incorporação das alterações é o pull request.

Uma pessoa responsável pelo projeto original irá receber seu pull request, analisá-lo e decidir o que fazer com o pedido. Ela pode aceitar as alterações e fazer o *pull* ou devolver a solicitação pedindo alguns ajustes.

<p style="text-align: center"><img src="/res/img/github/pull-request.png" alt="Imagem representativa de um pull request no Git." title="Pessoa fazendo o pull request das alterações de um projeto para o projeto original no Git." style="margin-top: 15px; margin-bottom: 15px;" /></p>

### <a name="merge"></a>Merge

Depois que você termina de trabalhar com um branch, você precisa incorporar as alterações deste branch para outro (normalmente o Master). Esta operação de incorporar um branch a outro se chama **merge**.

<p style="text-align: center"><img src="/res/img/github/merge.png" alt="Imagem representativa de um merge no Git." title="Pessoa fazendo o merge das alterações de um branch para o Master no Git." style="margin-top: 15px; margin-bottom: 15px;" /></p>

O merge evita que todas as alterações feitas em um branch precisem ser replicadas manualmente para outro branch. Esta operação também permite que alguém revise a junção das alterações entre os branches, antes de enviar para o Master.

Pense no Master e nos branches como se você estivesse trabalhando paralelamente em duas versões diferentes do mesmo projeto. Eventualmente, você precisará juntar as alterações feitas em uma versão (branch) com a versão principal (Master). O *merge* é esta ação de juntar as duas versões.

<p style="text-align: center"><img src="/res/img/github/merge-exemplo.png" alt="Imagem representativa de um merge no Git." title="Linha do tempo demonstrando a operação de juntar as alterações de um branch paralelo com o Master no Git." style="margin-top: 15px; margin-bottom: 15px;" /></p>

Quando se trabalha em equipe, é possível que você precise enviar um pedido de Merge para alguém aprovar — este processo é chamado de **merge request**. Outra pessoa irá revisar o *merge request* antes de aceitar as alterações e incorporá-las no Master.

## <a name="tracked-vs-untracked-versionado-e-não-versionado"></a>Tracked vs. Untracked (Versionado e não versionado)

**Tracked** e **untracked** são as situações em que um arquivo se encontra no seu working copy.

* **Untracked** é a situação de novos arquivos que você cria no working copy e que ainda não foram enviados para o repositório. Portanto, o arquivo ainda não está versionado; o arquivo ainda não está sob domínio do controle de versão.
* **Tracked** é as situação de arquivos que já foram enviados do working copy para o repositório. Ou seja, arquivos que já estão passando pelo controle de versão e têm suas alterações detectadas pelo sistema.

<p style="text-align: center"><img src="/res/img/github/tracked-untracked.png" alt="Imagem representativa de arquivos versionados e não versionados." title="Pessoa fazendo o push de um arquivo para o repositório remoto, tornando o arquivo versionado." style="margin-top: 15px; margin-bottom: 15px;" /></p>

Ao trabalhar com controle de versão, você deve querer que *todo* o seu projeto esteja **versionado**. Só assim você garante que está tudo guardado no repositório e pronto para ser editado por toda a equipe.

## <a name="docs-as-code"></a>Docs-as-code

**Docs-as-code** ("documentação como código") é o conceito de trabalhar com múltiplas revisões da documentação e versioná-la. É a metodologia de trabalho onde a documentação fica num repositório e está sob um controle de versão, assim como o código-fonte do software. Com a metodologia docs-as-code, a documentação passa por todas as operações explicadas aqui na página de terminologias.

---

O tópico [Enviar uma contribuição](/tutoriais/github/enviar-contribuicao/) demonstra como os conceitos desses termos se aplicam na prática do fluxo de contribuição.

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/github/fluxo-contribuicao/"><button type="button" class="btn btn-dark">Fluxo de contribuição</button></a></p>
