---
layout: curso-modulo-2
title: Organizando documentos extensos
permalink: /curso/modulo-2/documentos-extensos/
---

# Organizando documentos extensos

<div class="alerta alerta-simples">
    <p>Tempo estimado: 20 minutos</p>
</div>

Como você organiza uma grande coleção de informações em um documento ou site coeso? Ou, como você reorganiza um documento ou site confuso existente em algo acessível e útil? As seguintes táticas podem ajudar:

* Optar por escrever um único documento grande ou um conjunto de documentos
* Organizar um documento
* Adicionar navegação
* Divulgar informações progressivamente

## Quando escrever documentos extensos

Você pode organizar uma coleção de informações em documentos independentes mais longos ou em um conjunto de documentos interconectados mais curtos. Um conjunto de documentos interconectados mais curtos é frequentemente publicado como um site, wiki ou formato estruturado semelhante.

Alguns leitores respondem mais positivamente do que outros a documentos mais longos. Considere as seguintes perspectivas de dois leitores hipotéticos para os quais você está escrevendo a documentação:

* Hugo acha a leitura de documentos longos difícil e desorientadora. Ele prefere usar a pesquisa do site para encontrar respostas para suas perguntas.
* Rosa se sente confortável navegando em documentos grandes. Ela costuma usar o recurso de pesquisa de página integrado em seu navegador da Web para encontrar informações úteis na página atual.

Então, você deve organizar seu material em um único documento ou em um conjunto de documentos em um site? Considere as seguintes diretrizes:

* Guias de instruções, visões gerais introdutórias e guias conceituais geralmente funcionam melhor como documentos mais curtos quando direcionados a leitores que são novos no assunto. Por exemplo, um leitor que é completamente novo em seu assunto pode ter dificuldade em lembrar muitos novos termos, conceitos e fatos. Lembre-se de que seu público pode estar lendo sua documentação para obter uma visão geral rápida e geral do tópico.
* Tutoriais aprofundados, guias de práticas recomendadas e páginas de referência de linha de comando podem funcionar bem como documentos mais longos, especialmente quando direcionados a leitores que já têm alguma experiência com as ferramentas e o assunto.
* Um ótimo tutorial pode contar com uma narrativa para conduzir o leitor por uma série de tarefas relacionadas em um documento mais longo. No entanto, mesmo tutoriais grandes podem, às vezes, se beneficiar ao serem divididos em partes menores.
* Muitos documentos mais longos não são projetados para serem lidos de uma só vez. Por exemplo, os usuários normalmente percorrem uma página de referência para procurar uma explicação de um comando ou indicador.

O restante desta unidade abrange técnicas que podem ser úteis para escrever documentos mais longos, como tutoriais e alguns guias conceituais.

## Organizar um documento

Esta seção sugere algumas técnicas para planejar um documento mais longo, incluindo a criação de um esboço e a redação de uma introdução. Depois de concluir o primeiro rascunho de um documento, você pode revisá-lo em relação ao esboço e à introdução para garantir que não tenha perdido nada do que pretendia originalmente cobrir.

### Criar esboço de um documento

Começar com uma estrutura de tópicos de alto nível pode ajudá-lo a agrupar tópicos e determinar onde mais detalhes são necessários. O esboço ajuda você a mover os tópicos antes de começar a escrever.

Você pode achar útil pensar em um esboço como a narrativa do seu documento. Não há uma abordagem padrão para escrever um esboço, mas as diretrizes a seguir fornecem dicas práticas que podem ser úteis:

* Antes de pedir ao seu leitor para realizar uma tarefa, explique-lhes por que eles estão fazendo isso. Por exemplo, os tópicos a seguir ilustram uma seção de um esboço de um tutorial sobre auditoria e melhoria da acessibilidade de páginas da web:
  * Introduza um plug-in de navegador que audite a acessibilidade das páginas da web; explique que o leitor usará os resultados do relatório de auditoria para corrigir vários bugs.
  * Liste as etapas para executar o plug-in e auditar a acessibilidade de uma página da web.
* Limite cada passo do seu esboço para descrever um conceito ou completar uma tarefa específica.
* Estruture seu esboço para que seu documento apresente informações quando forem mais relevantes para o leitor. Por exemplo, seu leitor provavelmente não precisa saber (ou querer saber) sobre a história do projeto nas seções introdutórias do seu documento quando está apenas começando com o básico. Se você achar que o histórico do projeto é útil, inclua um link para esse tipo de informação no final do documento.
* Considere explicar um conceito e, em seguida, demonstrar como o leitor pode aplicá-lo em um projeto de amostra ou em seu próprio trabalho. Documentos que alternam entre informações conceituais e etapas práticas podem ser uma maneira particularmente atraente de aprender.
* Antes de começar a redigir, compartilhe o esboço com seus colaboradores. Os esboços são especialmente úteis se você estiver trabalhando com uma equipe de colaboradores que irão revisar e testar seu documento.

#### **Exercício: criando um esboço**

Revise e atualize o seguinte esboço geral de uma introdução a um longo tutorial. Para resolver este exercício, você pode fazer o seguinte:

* Reorganizar os tópicos existentes.
* Adicionar os tópicos ausentes que você acha que deveriam estar em uma introdução.
* Remover quaisquer tópicos que você considere irrelevantes para uma introdução.

>```text
>## História do projeto
>Descreve a história do desenvolvimento do projeto.
>## Pré-requisitos
>Lista conceitos com os quais o leitor deve estar familiarizado antes de começar, bem como quaisquer requisitos de software ou hardware.
>## Design do sistema
>Descreve como o sistema funciona.
>## Público
>Descreve a quem o tutorial se destina.
>## Configurando o tutorial
>Explica como configurar seu ambiente para seguir o tutorial.
>## Solução de problemas
>Explica como diagnosticar e resolver problemas potenciais que podem ocorrer enquanto o leitor segue o tutorial.
>## Terminologia útil
>Lista definições de termos que o leitor precisa saber para seguir o tutorial.
>```

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Segue uma possível solução:</p>

<blockquote>
<code>
<p>## Público</p>
<p>Descreve a quem o tutorial se destina.</p>
<p>## Pré-requisitos</p>
<p>Lista conceitos com os quais o leitor deve estar familiarizado antes de começar, bem como quaisquer requisitos de software ou hardware.</p>
<p>## Configurando o tutorial</p>
<p>Explica como configurar seu ambiente para seguir o tutorial.</p>
<p>## Terminologia útil</p>
<p>Lista definições de termos que o leitor precisa saber para seguir o tutorial.</p>
</code>
</blockquote>

</details>

### Criar uma introdução para um documento

Se os leitores de sua documentação não acharem o assunto relevante, provavelmente o ignorarão. Para definir as regras básicas para seus usuários, recomendamos escrever uma introdução que inclua as seguintes informações:

* O que o documento cobre.
* Que conhecimento prévio você espera que os leitores tenham.
* O que o documento não cobre.

Lembre-se de que você precisa que sua documentação seja fácil de manter, portanto, não tente cobrir tudo na introdução.

O parágrafo a seguir demonstra as ideias da lista anterior como uma visão geral para uma plataforma hipotética de publicação de documentos chamada Froobus:

> Este documento explica como publicar arquivos Markdown usando o sistema Froobus.
> Froobus é um sistema de publicação que roda em um servidor Linux e converte
> aquivos Markdown em páginas HTML. Este documento destina-se a pessoas que estão
> familiarizadas com a sintaxe Markdown. Para saber mais sobre a sintaxe, consulte as
> referências sobre Markdown. Você também precisa se sentir confortável executando comandos simples
> em um terminal Linux. Este documento não inclui informações sobre instalação ou como
> configurar um sistema de publicação Froobus. Para obter informações sobre a instalação do Froobus,
> consulte o tópico de Primeiros Passos.

Depois de concluir o primeiro rascunho, verifique todo o documento em relação às expectativas estabelecidas no texto introdutório. Sua introdução dá uma visão geral e precisa dos tópicos que você cobre? Você pode achar útil pensar nesta revisão como uma forma de garantia de qualidade da documentação (QA).

#### **Exercício: revisando uma introdução**

Para este exercício, revise a introdução a seguir sobre um guia de práticas recomendadas para uma linguagem de programação hipotética chamada F@. Remova qualquer informação que você considere irrelevante neste contexto e adicione qualquer informação que você ache que está faltando.

> Este guia lista as melhores práticas para trabalhar com a linguagem de programação F@.
> F@ foi desenvolvido em 2011 como um projeto comunitário de código aberto. Este guia
> complementa o guia de estilo F@. Além das práticas recomendadas neste guia,
> certifique-se de instalar também o linter de linha de comando F@ e de executá-lo em seu código.
> A linguagem de programação é amplamente adotada na indústria da saúde. Se você tiver
> sugestões para adições à lista de melhores práticas, registre uma *issue* no
> repositório de documentação F@.

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Segue uma possível solução:</p>

<blockquote>
<p>Este guia lista as melhores práticas para trabalhar com a linguagem de programação F@. Antes de revisar este guia, conclua o tutorial introdutório para novos desenvolvedores em F@. Este guia complementa o guia de estilo F@. Além das práticas recomendadas neste guia, certifique-se de instalar também o linter de linha de comando F@ e de executá-lo em seu código. Se você tiver sugestões para adições à lista de melhores práticas, registre uma <i>issue</i> no repositório de documentação F@.</p>
</blockquote>

</details>

## Adicionar navegação

Fornecer navegação e sinalização para seus leitores garante que eles possam encontrar o que estão procurando e as informações de que precisam para se libertar.

A navegação clara inclui:

* seções de introdução e sumário
* um desenvolvimento claro e lógico do assunto
* títulos e subtítulos que ajudam os usuários a entenderem o assunto
* um menu de índice (*table of contents*) que mostra aos usuários onde eles estão no documento
* links para recursos relacionados ou informações mais detalhadas
* links para o que aprender a seguir

As dicas nas seções a seguir podem ajudá-lo a planejar os títulos em sua documentação.

### Prefira títulos baseados em tarefas

Escolha um título que descreva a tarefa em que seu leitor está trabalhando. Evite títulos que dependem de terminologia ou ferramentas desconhecidas. Por exemplo, suponha que você esteja documentando o processo de criação de um novo site. Para criar o site, o leitor deve inicializar o framework Froobus. Para inicializar o framework Froobus, o leitor deve executar a ferramenta de linha de comando `carambola`. À primeira vista, pode parecer lógico adicionar um dos seguintes títulos às instruções:

* Executando o comando `carambola`
* Inicializando o framework Froobus

Mas, a menos que seus leitores já tenham muita experiência com a terminologia e os conceitos deste tópico, um título mais familiar pode ser preferível, como *Criando o site*.

### Forneça um texto em cada título

A maioria dos leitores aprecia pelo menos uma breve introdução em cada título para fornecer algum contexto. Evite colocar um título de nível três imediatamente após um título de nível dois, como no exemplo a seguir:

>```text
>## Criando o site
>### Executando o comando `carambola`
>```

Neste exemplo, uma breve introdução pode ajudar a orientar o leitor:

>```text
>## Criando o site
>
>Para criar o site, você executa a ferramenta de linha de comando `carambola`. O comando
>exibe uma série de prompts para ajudá-lo a configurar o site.
>
>### Executando o comando `carambola`
>```

#### **Exercício: cabeçalhos/subtítulos**

Ajudar os leitores a navegar pela documentação os ajuda a encontrar as informações de que precisam para usar sua ferramenta com sucesso. Muitas vezes, um sumário ou esquema claro e bem organizado funciona como um mapa que ajuda seus usuários a navegar pela funcionalidade de sua ferramenta.

Para este exercício, melhore o esboço a seguir. Você pode reorganizar, adicionar e excluir tópicos e também criar entradas secundárias.

> Sobre este tutorial
> Tópicos avançados
> Construir a árvore de navegação de recursos
> Definir caminhos de recursos
> Definindo e construindo projetos
> Iniciar o ambiente de desenvolvimento
> Definindo e construindo recursos
> O que vem a seguir
> Definir recursos de imagem
> Público
> Veja também
> Criar um recurso de imagem
> Definir um projeto de imagem
> Construir um projeto de imagem
> Configurando o tutorial
> Selecionar a raiz dos recursos do tutorial
> Sobre este guia

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Segue uma possível solução:</p>

<blockquote>
<p>## Sobre este tutorial</p>
<p>### Público</p>
<p>### Sobre este guia</p>
<p>### Tópicos avançados</p>
<p>## Configurando o tutorial</p>
<p>### Selecionar a raiz dos recursos do tutorial</p>
<p>### Iniciar o ambiente de desenvolvimento</p>
<p>### Construir a árvore de navegação de recursos</p>
<p>### Definir caminhos de recursos</p>
<p>## Definindo e construindo recursos</p>
<p>### Definir recursos de imagem</p>
<p>### Construir um projeto de imagem</p>
<p>## Definindo e construindo projetos</p>
<p>### Definir um projeto de imagem</p>
<p>### Construir um projeto de imagem</p>
<p>## Definindo e construindo bancos de dados</p>
<p>### Definir um banco de dados</p>
<p>### Construir um banco de dados</p>
<p>## Enviando, publicando e consultando um banco de dados</p>
<p>### Enviar um banco de dados</p>
<p>### Publicar um banco de dados</p>
<p>### Consultar um banco de dados</p>
<p>## Configurando regras de visualização para dados vetoriais</p>
<p>### Definir, configurar e construir dados vetoriais</p>
<p>## Veja também</p>
<p>### Exemplos de arquivos de dados</p>
<p>## O que vem a seguir</p>
</blockquote>

</details>

### Dê informações progressivamente

Aprender novos conceitos, ideias e técnicas pode ser uma experiência gratificante para muitos leitores que se sentem à vontade para ler a documentação em seu próprio ritmo. No entanto, ser confrontado com muitos novos conceitos e instruções muito rapidamente pode ser esmagador. Os leitores são mais propensos a serem receptivos a documentos mais longos que progressivamente divulgam novas informações a eles quando precisam. As técnicas a seguir podem ajudá-lo a incorporar a divulgação progressiva em seus documentos:

* Sempre que possível, tente introduzir novas terminologias e conceitos próximos às instruções que se baseiam neles.
* Quebre grandes "blocões de texto". Para evitar vários parágrafos grandes em uma única página, tente introduzir tabelas, diagramas, listas e títulos quando apropriado.
* Quebre uma grande série de etapas. Se você tiver uma lista particularmente longa de etapas complicadas, tente reorganizá-las em listas mais curtas que explicam como concluir subtarefas.
* Comece com exemplos e instruções simples e adicione técnicas progressivamente mais interessantes e complicadas. Por exemplo, em um tutorial para criar formulários, comece explicando como lidar com respostas de texto e, em seguida, apresente outras técnicas para lidar com múltipla escolha, imagens e outros tipos de resposta.

---

<p class="proxima-unidade"><b>Próxima unidade:</b> <a href="/curso/modulo-2/ilustracoes/"><button type="button" class="btn btn-dark">Ilustrações</button></a></p>

{% include footer-conteudo-traduzido.html %}
