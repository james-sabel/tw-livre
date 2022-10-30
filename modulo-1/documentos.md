---
layout: curso-modulo-1
title: Documentos
permalink: /curso/modulo-1/documentos/
---

# Documentos

<div class="alerta alerta-simples">
    <p>Tempo estimado: 10 minutos</p>
</div>

Você pode escrever frases. Você pode escrever parágrafos. Mas você consegue organizar todos esses parágrafos em um documento coerente?

## Defina o escopo do seu documento

Um bom documento começa definindo seu escopo. Por exemplo:

> Este documento descreve o design do Projeto Frambus.

Um documento melhor define também o que não está no escopo – tópicos não cobertos, mas que seria razoável assumir que o público-alvo espera que seu documento abranja. Por exemplo:

> Este documento não descreve o projeto para a tecnologia relacionada, Projeto Froobus.

As definições de escopo e não escopo beneficiam não apenas o leitor, mas também o redator (você). Ao escrever, se o conteúdo do seu documento se desviar da definição de escopo (ou se aventurar na declaração de não escopo), você deve redirecionar seu documento ou modificar sua definição de escopo. Ao revisar seu primeiro rascunho, exclua todas as seções que não ajudam a atender a definição de escopo.

### Exercício

Que problema você vê no parágrafo a seguir?

> Este documento explica como usar a API do Frambus para criar, atualizar e publicar Fwidgets. Este documento não explica como usar a API do Frambus para excluir Fwidgets ou cobrir a história do sistema operacional Linux.

<details>
<summary>Clique para revelar a resposta.</summary>

<p>O não escopo deve incluir apenas informações que os usuários razoavelmente esperariam que o documento abrangesse. A julgar pela primeira frase, nenhum usuário razoável esperaria que o documento cobrisse a história do sistema operacional Linux.</p>

</details>

## Defina seu público

Um bom documento especifica explicitamente seu público. Por exemplo:

> Este documento destina-se aos seguintes públicos:
>
> * Engenheiros de software
> * Gerentes de projeto

Além do papel do público, uma boa declaração do público também pode especificar qualquer pré-requisito de conhecimento ou experiência. Por exemplo:

> Este documento pressupõe que você entenda a multiplicação de matrizes e os fundamentos da retropropagação.

Em alguns casos, a declaração do público também deve especificar a leitura ou o curso pré-requisito. Por exemplo:

> Você deve ler o "Projeto Froobus: Uma Nova Esperança" antes de ler este documento.

## Resuma os pontos-chave no início

Engenheiros e cientistas são pessoas ocupadas que não necessariamente lerão todas as 76 páginas do seu documento de projeto. Imagine que seus colegas possam ler apenas o primeiro parágrafo do seu documento. Portanto, certifique-se de que o início do seu documento responda às perguntas essenciais de seus leitores.

Redatores profissionais concentram uma energia considerável na primeira página para aumentar as chances de os leitores chegarem à segunda página. No entanto, o início de qualquer documento longo é a página mais difícil de escrever. Esteja preparado para revisar a primeira página muitas vezes.

### Faça comparações e dê contrastes

Em sua carreira, não importa o quão criativo você seja, você criará poucos documentos preciosos contendo ideias verdadeiramente revolucionárias. A maior parte do seu trabalho será evolucionária, baseada em tecnologias e conceitos existentes. Portanto, compare e contraste suas ideias com conceitos que seu público já entende. Por exemplo:

> Este novo aplicativo é semelhante ao aplicativo Frambus, mas com gráficos melhores.

Ou:

> A API Froobus lida com os mesmos casos de uso que a API Frambus, mas que a API Froobus é mais fácil de usar.

### Exercício

Que problema você vê na introdução a seguir?

> O aplicativo Frambus Weather v2 apresenta dez recursos que não estão disponíveis no aplicativo Frambus Weather v1. Mais importante ainda, a v2 oferece previsões de duas semanas; a v1 oferece previsões de apenas uma semana. As informações sobre marés não sofreram alterações.

<details>
<summary>Clique para revelar a resposta.</summary>

<p>A frase final (sobre marés) não é importante o suficiente para aparecer no parágrafo de abertura. A primeira frase mencionou dez novos recursos, então os leitores provavelmente esperariam ouvir mais sobre esses novos recursos. Em vez disso, a frase final refere-se a algo diferente de um novo recurso.</p>

</details>

## Escreva para o seu público

Este curso enfatiza repetidamente a importância de definir seu público. Nesta seção, nos concentramos na definição de público como meio de organizar seu documento.

### Defina as necessidades do seu público

Responder às seguintes perguntas ajuda a determinar o que seu documento deve conter:

* Quem é seu público-alvo?
* Qual é o objetivo do seu público-alvo? Por que eles estão lendo este documento?
* O que seus leitores já sabem *antes* de ler seu documento?
* O que seus leitores devem saber ou ser capazes de fazer *depois* de lerem seu documento?

Por exemplo, suponha que você tenha inventado um novo algoritmo de ordenação, semelhante ao *quicksort*. A lista a seguir contém algumas respostas possíveis para as perguntas anteriores:

* **Quem é seu público-alvo?** O público-alvo consiste em todos os engenheiros de software da minha organização.
* **Qual é o objetivo do seu público-alvo?** Meu público-alvo deseja encontrar maneiras mais eficientes de ordenar dados. Eles estão lendo este documento para determinar se vale a pena implementar esse novo algoritmo.
* **O que seus leitores já sabem antes de ler seu documento?** Meu público-alvo sabe escrever código e já estudou algoritmos de ordenação, incluindo *quicksort*. No entanto, a maioria das pessoas do meu público-alvo não implementa ou avalia um algoritmo de ordenação há vários anos.
* **O que seus leitores devem saber ou ser capazes de fazer depois de lerem seu documento?** Meu público-alvo será capaz de fazer o seguinte:
  * Entender como o algoritmo se compara e contrasta com o *quicksort*.
  * Identificar os dois tipos de conjuntos de dados para os quais o algoritmo supera o algoritmo *quicksort*.
  * Implementar o algoritmo na linguagem de programação de sua escolha.
  * Identificar os dois casos extremos em que o algoritmo tem um desempenho ruim.

### Organize o documento para atender às necessidades do seu público

Depois de definir as necessidades do público, organize o documento para ajudar os leitores a obter as informações de que precisam. Por exemplo, com base nas respostas da seção anterior, o esboço do documento pode ter a seguinte aparência:

1. Visão geral do algoritmo
* Comparação e contraste com *quicksort*, incluindo comparações com O-grande
  * Link para o artigo da Wikipedia sobre *quicksort*
* *Datasets* ideais para o algoritmo

2. Implementando o algoritmo
  * Implementação em pseudocódigo
  * Dicas de implementação, incluindo erros comuns

3. Análise mais profunda do algoritmo
  * Casos extremos
  * Problemas conhecidos

---

<p class="proxima-unidade"><b>Próxima unidade:</b> <a href="/curso/modulo-1/pontuacao/"><button type="button" class="btn btn-dark">Pontuação</button></a> (opcional)</p>

{% include footer-conteudo-traduzido.html %}
