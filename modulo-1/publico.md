---
layout: curso-modulo-1
title: Público
permalink: /curso/modulo-1/publico/
---

# Público

<div class="alerta alerta-simples">
    <p>Tempo estimado: 10 minutos</p>
</div>

Esta unidade começa com uma equação: (Por favor, não se assuste se você não se sentir à vontade com a matemática.)

> boa documentação = conhecimento e habilidades que seu público precisa para completar uma tarefa − o conhecimento e as habilidades atuais do seu público

Em outras palavras, certifique-se de que seu documento forneça as informações que seu público precisa, mas que ainda não possui. Portanto, esta unidade explica como fazer o seguinte:

* Definir seu público.
* Determinar o que seu público precisa aprender.
* Ajustar a documentação ao seu público.

Como o vídeo a seguir sugere, segmentar o público errado pode ser confuso:

<iframe width="560" height="315" src="https://www.youtube.com/embed/eFtXIrmsMwI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

***Descrição do vídeo para acessibilidade:** o vídeo mostra um homem num palco de teatro, com trajes de época e recitando passagens de Shakespeare. Enquanto ele recita, a câmera mostra o público do teatro assistindo atentamente. Em seguida, o vídeo alterna para um grupo de adolescentes rindo e mostrando a língua num campo esportivo. O vídeo mostra a frase "combine o seu conteúdo com o seu público". Por fim, a imagem volta para o teatro e mostra o público aplaudindo.*

## Defina seu público

Uma documentação feita com esforço investe tempo e energia consideráveis ​​na definição de seu público. Esses esforços podem envolver pesquisas, estudos de experiência do usuário, grupos focais e testes de documentação. Você provavelmente não tem todo esse tempo, então esta unidade adota uma abordagem mais simples.

Comece identificando o(s) papel(éis) do seu público. Estes são alguns papéis de exemplo:

* engenheiros de software
* cargos técnicos, não de engenharia (como gerentes de projeto técnicos)
* cientistas
* profissionais em áreas científicas (por exemplo, médicos)
* estudantes de engenharia
* formados em engenharia
* cargos não técnicos

É de se reconhecer que muitas pessoas em cargos não técnicos tenham grandes habilidades técnicas e matemáticas. No entanto, os papéis continuam sendo uma primeira aproximação essencial na definição de seu público. Pessoas dentro do mesmo papel geralmente compartilham certas habilidades e conhecimentos básicos. Por exemplo:

* A maioria dos engenheiros de software conhece algoritmos de ordenação populares, [notação O-grande](https://pt.wikipedia.org/wiki/Grande-O) e pelo menos uma linguagem de programação. Portanto, você pode contar que engenheiros de software sabem o que O(n) significa, mas não pode contar que pessoas de cargos não técnicos conheçam O(n).
* Um relatório de pesquisa direcionado a médicos deve ser muito diferente de um artigo de jornal sobre a mesma pesquisa destinada a um público leigo.
* A explicação de um professor sobre uma nova abordagem de *machine learning* para alunos de pós-graduação deve ser diferente da explicação para alunos de graduação do primeiro semestre.

Escrever seria muito mais fácil se todos no mesmo papel compartilhassem exatamente o mesmo conhecimento. Infelizmente, o conhecimento dentro do mesmo papel diverge. Mauro é especialista em Python, Sharlene é especialista em C++ e Michel em Java. Karine adora Linux, mas Davi só conhece iOS.

Os papéis, por si só, são insuficientes para definir um público. Ou seja, você também deve considerar a proximidade do seu público com o tema. Os engenheiros de software do Projeto Frombus sabem alguma coisa sobre o Projeto Dingus, os quais estão relacionados, mas nada sabem sobre o Projeto Carambola, com o qual não estão relacionados. O cardiologista médio sabe mais sobre problemas de ouvido do que o engenheiro de software médio, mas sabe muito menos do que um fonoaudiólogo.

O tempo de experiência também afeta a afinidade. Quase todos os engenheiros de software, por exemplo, estudaram cálculo. No entanto, a maioria dos engenheiros de software não usa cálculo em seus trabalhos, então seu conhecimento de cálculo desaparece gradualmente. Por outro lado, engenheiros experientes normalmente sabem muito mais sobre seu projeto atual do que novos engenheiros no mesmo projeto.

## Exemplo de análise de público

A seguir, um exemplo de análise de público para o fictício Projeto Zylmon:

> O público do Projeto Zylmon se enquadra nos seguintes papéis:
>
> * engenheiros de software
> * gerentes técnicos de produto
>
> O público tem a seguinte familiaridade com o tema:
>
> * Meu público já conhece as APIs do Zyljeune, que são um pouco semelhantes às APIs do Zylmon.
> * Meu público conhece C++, mas normalmente não construiu programas C++ no novo ambiente de desenvolvimento Vitória Alada.
> * Meu público estudou álgebra linear na universidade, mas muitos membros da equipe precisam de uma atualização sobre multiplicação de matrizes.

## Determine o que seu público precisa aprender

Anote uma lista de tudo o que seu público precisa aprender para atingir objetivos. Em alguns casos, a lista deve conter tarefas que o público precisa realizar. Por exemplo:

> Após a leitura da documentação, o público saberá como realizar as seguintes tarefas:
>
> * Usar a API do Zylmon para listar hotéis por preço.
> * Usar a API do Zylmon para listar hotéis por localização.
> * Usar a API do Zylmon para listar hotéis por classificações de usuários.

Observe que, às vezes, seu público deve dominar as tarefas em uma determinada ordem. Por exemplo, seu público pode precisar aprender a construir e executar programas em um novo ambiente de desenvolvimento antes de aprender a escrever tipos específicos de programas.

Se você estiver escrevendo uma especificação de design, sua lista deve se concentrar nas informações que seu público deve aprender, em vez de dominar tarefas específicas. Por exemplo:

> Depois de ler as especificações de design, o público aprenderá o seguinte:
>
> * Três razões pelas quais Zylmon supera Zyljeune.
> * Cinco razões pelas quais o Zylmon consumiu 5,25 anos de engenharia para ser desenvolvido.

## Ajuste a documentação ao seu público

Escrever para atender às necessidades do seu público requer empatia. Você deve criar explicações que satisfaçam a curiosidade do seu público e não a sua. Como fazer para sair de si mesmo para adequar a documentação ao público? Infelizmente, não podemos oferecer respostas fáceis. Podemos, no entanto, oferecer alguns pontos de atenção.

### Vocabulário e conceitos

Combine seu vocabulário com o seu público. Leia o tópico [Palavras](/curso/modulo-1/palavras/) para obter ajuda.

Esteja atento às afinidades. As pessoas de sua equipe provavelmente entendem as abreviações de sua equipe, mas será que as pessoas de outras equipes entendem essas mesmas abreviações? À medida que seu público se amplia, assuma que você deve explicar mais.

Da mesma forma, pessoas experientes em sua equipe de software provavelmente entendem os detalhes de implementação e as estruturas de dados do projeto de sua equipe, mas quase todo mundo (incluindo novos membros de sua equipe) não. A menos que você esteja escrevendo especificamente para outros membros experientes de sua equipe, normalmente você deve explicar mais do que espera.

### Maldição do conhecimento

Os especialistas geralmente sofrem com **a maldição do conhecimento**, o que significa que sua compreensão especializada de um tópico arruína suas explicações para os recém-chegados. Como especialistas, é fácil esquecer que os novatos não sabem o que você já sabe. Os novatos podem não entender explicações que fazem referência passageira a interações sutis e sistemas aprofundados que o especialista não para para explicar.

Do ponto de vista do novato, a maldição do conhecimento é um erro de "Arquivo não encontrado" causado por um módulo ainda não compilado.

#### Exercício

1. Suponha que o parágrafo a seguir seja o início de um artigo destinado a médicos que nunca programaram antes. Identifique os aspectos do parágrafo que sofrem com a maldição do conhecimento:

  > C é uma linguagem de nível médio, superior à linguagem assembly, mas inferior ao Python e ao Java. A linguagem C fornece aos programadores controle refinado sobre todos os aspectos de um programa. Por exemplo, usando a biblioteca padrão de C, é fácil alocar e liberar blocos de memória. Em C, manipular ponteiros diretamente é mundano.

2. Suponha que o parágrafo anterior fosse destinado a estudantes de graduação em ciência da computação iniciantes em C, mas familiarizados com Python. O parágrafo ainda sofre com a maldição do conhecimento?

<details>
<summary>Clique para revelar a resposta.</summary>

<ol>
  <li>Este parágrafo sofre imensamente com a maldição do conhecimento. O público-alvo nunca programou antes, portanto, os seguintes termos são inadequados ou desconhecidos:
    <ul>
      <li>linguagem</li>
      <li>linguagem de nível médio</li>
      <li>linguagem de montagem</li>
      <li>Python</li>
      <li>Java</li>
      <li>programa</li>
      <li>biblioteca padrão de C</li>
      <li>alocar e liberar blocos de memória</li>
      <li>ponteiros</li>
    </ul>
  </li>
  <li>Este parágrafo também sofre com a maldição do conhecimento para o público alternativo. O programador Python médio não tem conhecimento de manipulação de memória ou ponteiros. Um parágrafo introdutório seria melhor se comparasse C com Python.</li>
</ol>

</details>

### Palavras simples, neutralidade cultural e expressões idiomáticas

Palavras difíceis e raras repelem alguns leitores, além de dificultarem a tradução para outros idiomas. Já as palavras simples facilitam a internacionalização da documentação. Portanto, prefira palavras simples a palavras complexas; evite palavras em português obsoletas ou excessivamente complexas.

Mantenha sua escrita culturalmente neutra. Não exija que os leitores entendam os pormenores da NASCAR, críquete ou sumô para entender como um software funciona.

**Expressões idiomáticas** são frases cujo significado geral difere do significado literal das palavras individuais dessa frase. A maioria dos leitores do Brasil reconhece essas expressões e maneiras de falar. No entanto, se você estiver escrevendo para um público internacional ou se a documentação for traduzida, substitua essas expressões por algo concreto.

As expressões idiomáticas estão tão profundamente enraizadas em nossa fala que o significado especial não literal das expressões idiomáticas se torna invisível para nós. Ou seja, as expressões idiomáticas são outra forma da maldição do conhecimento.

Observe que algumas pessoas em seu público usam software de tradução para ler sua documentação. O software de tradução tende a sofrer mais com referências culturais e expressões idiomáticas do que com o português simples.

---

<p class="proxima-unidade"><b>Próxima unidade:</b> <a href="/curso/modulo-1/documentos/"><button type="button" class="btn btn-dark">Documentos</button></a></p>

{% include footer-conteudo-traduzido.html %}
