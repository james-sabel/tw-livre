---
layout: curso-modulo-2
title: Trabalhando com ilustrações
permalink: /curso/modulo-2/ilustracoes/
---

# Ilustrações

<div class="alerta alerta-simples">
    <p>Tempo estimado: 10 minutos</p>
</div>

Lembra quando seu professor lhe deu um capítulo pesado para ler? Você folheou a seção designada do livro, esperando desesperadamente por... sim, fotos! Ver ilustrações era muito mais divertido do que ler texto. Na verdade, quando se trata de ler material técnico, a grande maioria dos adultos ainda são crianças – ainda anseiam por imagens em vez de texto.

<img src="/res/img/curso/book_readers.jpg" alt-text="Imagem - foto" title="Foto de três crianças sentadas no chão, em círculo, olhando e apontando para livros e revistas." class="imagem-curso" />

**Figura 1. Boas ilustrações engajam leitores de formas que o texto não consegue.**

*Créditos da imagem: [Nirmal Dulal](https://commons.wikimedia.org/wiki/File:Nepalese_Children.JPG)* - Domínio Público

De acordo com pesquisas de [Sung e Mayer (2012)](https://www.sciencedirect.com/science/article/pii/S0747563212000921), fornecer qualquer gráfico – bons ou ruins – faz com que os leitores gostem mais do documento; no entanto, apenas gráficos instrutivos ajudam os leitores a aprender. Esta unidade sugere algumas maneiras de ajudá-lo a criar figuras que realmente valem mais que mil palavras.

## Escreva a legenda primeiro

Muitas vezes é útil escrever a legenda antes de criar a ilustração. Em seguida, crie a ilustração que melhor representa a legenda. Esse processo ajuda você a verificar se a ilustração corresponde ao objetivo.

Boas legendas têm as seguintes características:

* Elas são **breves**. Normalmente, uma legenda é formada por apenas algumas palavras.
* Elas explicam a **ideia principal**. Depois de ver este gráfico, o que o leitor deve se lembrar?
* Elas **focam** a atenção do leitor. O foco é particularmente importante quando uma fotografia ou diagrama contém muitos detalhes.

<div class="alerta alerta-azul">
    <p>Por convenção, a legenda segue aparece seguinte ao diagrama.</p>
</div>

### Exercício

Público-alvo: Estudantes de graduação em Ciências da Computação que cursam uma aula de "Introdução a Estruturas de Dados".

Considere as três figuras a seguir, cada uma delas usando a mesma legenda.

<img src="/res/img/curso/caption_exercise_chain_a.svg" alt-text="Imagem - diagrama" title="Desenho de uma corrente multicolorida." class="imagem-curso" />

**Legenda A. Uma lista de links únicos abriga conteúdo e um ponteiro para o próximo nó (*node*).**

<img src="/res/img/curso/caption_exercise_drawing_b.png" alt-text="Imagem - diagrama" title="Desenho de quatro caixas conectadas por três setas." class="imagem-curso" />

**Legenda B. Uma lista de links únicos abriga conteúdo e um ponteiro para o próximo nó (*node*).**

<img src="/res/img/curso/caption_exercise_drawing_c.svg" alt-text="Imagem - diagrama" title="Desenho de quatro caixas (cada uma com conteúdo e um ponteiro) conectadas por três setas." class="imagem-curso" />

**Legenda C. Uma lista de links únicos abriga conteúdo e um ponteiro para o próximo nó (*node*).**

Qual das três figuras anteriores ilustra melhor sua legenda?

<details>
<summary>Clique para revelar a resposta.</summary>

<ul>
  <li>A figura A é ruim. A corrente é bonita, mas livre de informações. A corrente também implica erroneamente que uma lista encadeada aponta tanto para trás quanto para frente.</li>
  <li>A figura B está boa. A ilustração ajuda os alunos a perceberem que o primeiro item aponta para o segundo item, o segundo aponta para o terceiro e assim por diante. No entanto, embora a legenda se refira ao conteúdo e a um ponteiro, a ilustração mostra ponteiros, mas não mostra conteúdo.</li>
  <li>A Figura C é a melhor escolha e a mais instrutiva. A ilustração delineia claramente a parte do conteúdo de cada nó da parte do ponteiro.</li>
</ul>

</details>

## Restrinja a quantidade de informações em um único desenho

Poucas tarefas intelectuais podem ser tão recompensadoras quanto estudar uma bela pintura, descobrindo gradualmente camadas de percepção e significado. As pessoas pagam um bom dinheiro para fazer exatamente isso nos museus de arte do mundo.

<img src="/res/img/curso/van_gogh.jpeg" alt-text="Imagem - foto" title="Imagem de uma pintura de Van Gogh." class="imagem-curso" />

**Figura 2. Você ficaria feliz em estudar esta pintura de Van Gogh.**

*Créditos da imagem: [Portrait of Pere Tanguy By Vincent van Gogh - Musée Rodin](https://commons.wikimedia.org/wiki/File:Van_Gogh_-_Portrait_of_Pere_Tanguy_1887-8.JPG)* - Domínio Público

Por outro lado, ilustrações técnicas altamente complexas como as seguintes tendem a desencorajar a maioria dos leitores:

<img src="/res/img/curso/overly_complex_diagram.svg" alt-text="Imagem - diagrama" title="Desenho de um diagrama com várias caixas, linhas pontilhadas e setas interligadas." class="imagem-curso" />

**Figura 3. Diagramas de blocos complexos sobrecarregam os leitores.**

Assim como você evita frases excessivamente longas, esforce-se para evitar a junção de muitos elementos visuais. Como regra geral, não coloque mais do que um parágrafo de informação em um único diagrama. (Uma regra prática alternativa é evitar ilustrações que exijam mais de cinco itens com marcadores para explicar.) Posso ouvir você dizendo: "Mas os sistemas técnicos da vida real podem ser muito mais complexos do que os mostrados na Figura 3". Você está correto, mas provavelmente não se sente inclinado a explicar sistemas complexos da vida real em um único parágrafo.

O truque para transformar a desordem visual em algo coerente e útil é organizar sistemas complexos em subsistemas, como os mostrados na figura a seguir:

<img src="/res/img/curso/subsystems.svg" alt-text="Imagem - diagrama" title="Desenho de um diagrama de subsistema." class="imagem-curso" />


**Figura 4. Um sistema complexo organizado em subsistemas.**

Depois de mostrar a "visão geral", forneça ilustrações separadas de cada subsistema.

<img src="/res/img/curso/subsystems_zoomed.svg" alt-text="Imagem - diagrama" title="Zoom do subsistema da Figura 4." class="imagem-curso" />

**Figura 5. Detalhe expandido para um subsistema de um sistema complexo.**

Alternativamente, comece com uma simples "imagem geral" e, em seguida, expanda gradualmente os detalhes em cada ilustração subsequente.

## Concentre a atenção do leitor

Quando confrontados com uma captura de tela complexa como a seguinte, os leitores lutam para determinar o que é relevante:

<img src="/res/img/curso/unfocused_screenshot.png" alt-text="Imagem - ilustração" title="Captura de tela sem nenhuma parte destacada." class="imagem-curso" />

**Figura 6. Os leitores não sabem no que focar.**

Adicionar uma dica visual, por exemplo, o oval vermelho na figura a seguir, ajuda os leitores a se concentrarem na seção relevante da captura de tela:

<img src="/res/img/curso/focused_screenshot.png" alt-text="Imagem - ilustração" title="Mesma captura de tela da Figura 6, mas com uma parte destacada em vermelho." class="imagem-curso" />

**Figura 7. Os leitores se concentram em uma forma que sai do padrão.**

Os textos explicativos são outra maneira de focar a atenção do leitor. Para fotos e arte de linha, um texto explicativo ajuda nossos olhos a encontrar o ponto certo para concentrar. Os textos explicativos nas imagens geralmente são melhores do que as explicações longas de parágrafos das imagens porque os textos explicativos concentram a atenção do leitor nos aspectos mais importantes da imagem. Então, em sua explicação, você pode se concentrar diretamente na parte relevante do diagrama, em vez de gastar tempo descrevendo de qual parte da imagem você está falando.

Na imagem de exemplo, o texto explicativo e a seta direcionam rapidamente o leitor para o objetivo.

<img src="/res/img/curso/moon_with_callout.png" alt-text="Imagem - ilustração" title="Foto de Phobos com uma seta apontando para um ponto específico." class="imagem-curso" />

**Figura 8. Um texto explicativo direciona os olhos dos leitores.**

*Créditos da imagem: [NASA / JPL-Caltech / University of Arizona](https://commons.wikimedia.org/wiki/File:Phobos_colour_2008.jpg)* - Domínio Público

## Ilustrar é re-ilustrar

Tal como acontece com a escrita, o primeiro rascunho de uma ilustração raramente é bom o suficiente. Revise suas ilustrações para esclarecer o conteúdo. Ao revisar, faça a si mesmo as seguintes perguntas:

* Como posso simplificar a ilustração?
* Devo dividir esta ilustração em duas ou mais ilustrações mais simples?
* O texto na ilustração é fácil de ler? O texto contrasta suficientemente com o fundo?
* Qual é a ideia principal?

Por exemplo, considere a evolução do mapa do metrô de Londres. Antes de 1931, o mapa do metrô foi desenhado em escala, completo com estradas acima do solo e linhas de metrô que se curvavam como os trilhos.

<img src="/res/img/curso/tube_1908.jpg" alt-text="Imagem - ilustração" title="Mapa de 1908 do metrô de Londres." class="imagem-curso" />

**Figura 9. Mapa de 1908 do metrô de Londres desenhado em escala com as estradas acima do solo.**

*Créditos da imagem: [Autor desconhecido](https://commons.wikimedia.org/wiki/File:Tube_map_1908.jpg)* - Domínio Público

Em 1931, Harry Beck foi pioneiro em um novo tipo de mapa de transporte público que simplificou o mapa mais antigo, removendo os marcadores acima do solo e removendo a escala. Em vez disso, seu projeto se concentrou no que realmente importava para as pessoas que usavam os mapas: ir da estação A à estação B. Mesmo com o sucesso de seu mapa de 1931, Beck ainda repetiu o diagrama por muitos anos para simplificar e esclarecer o mapa. Considere agora o [mapa do metrô moderno](https://www.google.com/search?tbm=isch&q=london+tube+map), embora novas linhas e estações tenham surgido, elas ainda permanecem próximas ao projeto de Beck.

### Exercício

Considere a seguinte ilustração original:

<img src="/res/img/curso/recursion1.svg" alt-text="Imagem - diagrama" title="Um diagrama complexo." class="imagem-curso" />

**Figura 10. Um diagrama complexo.**

A conclusão do diagrama anterior deve ser:

> Para uma solução recursiva, chame a própria função na instrução `return` até chegar a uma solução de caso base.

De que forma a complexidade do diagrama esconde a ideia principal? Como você pode resolver esses problemas?

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Alguns possíveis problemas com o diagrama incluem:</p>

<ul>
    <li><b>Problema:</b> As cores brilhantes desviam a atenção do leitor de outros aspectos do diagrama.<br />
    <b>Solução:</b> Escolha as cores com cuidado para que não sobrecarreguem o diagrama.</li>
    <li><b>Problema:</b> O diagrama não tem contraste de cores suficiente. Isso torna o diagrama inacessível para algumas pessoas com baixa visão ou certos tipos de daltonismo.<br />
    <b>Solução:</b> remova o uso desnecessário de cores e certifique-se de que as cores atendam às recomendações padrão de contraste de cores.</li>
    <li><b>Problema:</b> As setas apontam em ambas as direções, o que deixa claro para que lado o diagrama flui.<br />
    <b>Solução:</b> Separe as setas em duas partes com um conjunto ilustrando a chamada de uma função e o outro conjunto ilustrando o retorno da função.</li>
</ul>

<p>Há problemas adicionais no diagrama que não são identificados aqui.</p>

</details>

Aqui está uma ilustração melhorada:

<img src="/res/img/curso/recursion2.svg" alt-text="Imagem - diagrama" title="Uma versão simplificada do diagrama anterior." class="imagem-curso" />

**Figura 11. Uma versão simplificada do diagrama anterior.**

Quais problemas você percebe na ilustração melhorada?

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Aqui estão duas das falhas que ainda existem:</p>

<ul>
    <li>Este diagrama ainda é muito complexo. Seria preciso muito mais do que um parágrafo para explicar essa ilustração. Considere como remover informações extras ou adicionar rótulos esclarecedores pode simplificar a interpretação.</li>
    <li>Embora a separação das setas ajude a exibir quando as funções invocam ou retornam dados umas às outras, as setas de retorno podem se beneficiar de rótulos que informam ao leitor quais são os valores de retorno.</li>
</ul>

</details>

## Ferramentas de ilustração

Há muitas opções disponíveis para criar diagramas. Três opções gratuitas ou com opções gratuitas incluem:

* [Google Drawings](https://drawings.google.com/)
* [diagrams.net](https://diagrams.net/)
* [LucidChart](https://www.lucidchart.com/pages/)

Ao exportar diagramas dessas ferramentas para uso na documentação, geralmente é melhor exportar os arquivos como Scalable Vector Graphics (SVG). O formato SVG dimensiona facilmente os diagramas com base nas restrições de espaço para que, independentemente do tamanho, você tenha uma imagem de alta qualidade.

---

<p class="proxima-unidade"><b>Próxima unidade:</b> <a href="/curso/modulo-2/codigo-exemplo/"><button type="button" class="btn btn-dark">Criando código de exemplo</button></a></p>

{% include footer-conteudo-traduzido.html %}
