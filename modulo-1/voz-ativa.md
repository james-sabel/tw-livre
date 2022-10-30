---
layout: curso-modulo-1
title: Voz ativa vs. voz passiva
permalink: /curso/modulo-1/voz-ativa/
---

# Voz ativa vs. voz passiva

<div class="alerta alerta-simples">
    <p>Tempo estimado: 15 minutos</p>
</div>

A grande maioria das frases na redação técnica deve estar na voz ativa. Esta unidade ensina como fazer o seguinte:

* Distinguir a voz passiva da voz ativa.
* Converter a voz passiva em voz ativa, porque a voz ativa geralmente é mais clara.

Primeiro, assista a este vídeo, apenas para dar o pontapé inicial [^1]:

<iframe width="560" height="315" src="https://www.youtube.com/embed/nG6DhoFt938" title="Vídeo do YouTube" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

***Descrição do vídeo para acessibilidade**: o vídeo começa mostrando a frase "Voz ativa: O jogador chuta a bola de futebol" e em seguida mostra um jogador em um campo de futebol, chutando uma bola. Depois, mostra a frase "Voz passiva: A bola de futebol é chutada pelo jogador" e em seguida a câmera está focada na bola sendo chutada.*

## Distinguir a voz ativa da voz passiva em frases simples

Em uma sentença de voz ativa, um ator faz uma ação com um alvo. Ou seja, uma sentença de voz ativa segue esta fórmula:

> Frase de voz ativa = ator + verbo + alvo

Uma frase na voz passiva inverte a fórmula. Ou seja, uma frase na voz passiva normalmente segue a seguinte fórmula:

> Frase de voz passiva = alvo + verbo + ator

### Exemplo de voz ativa

Por exemplo, aqui está uma frase de voz curta e ativa:

> O gato devorou a ração.

* ator: gato
* verbo: devorou
* alvo: ração

### Exemplos de voz passiva

Por outro lado, aqui está a mesma frase na voz passiva:

> A ração foi devorada pelo gato.

* alvo: ração
* verbo passivo: devorada
* ator: gato

Algumas frases de voz passiva omitem um ator. Por exemplo:

> A ração foi devorada.

* ator: *desconhecido*
* verbo passivo: foi devorada
* alvo: ração

Quem ou o que devorou a ração? Um gato? Um cachorro? Um T-Rex? Os leitores teriam que adivinhar. Boas frases na documentação técnica identificam quem está fazendo o que para quem.

## Reconhecer verbos passivos

Os verbos passivos geralmente têm a seguinte fórmula:

> verbo passivo = forma de ser + verbo no particípio passado

Embora a fórmula anterior pareça assustadora, na verdade é bem simples:

* Uma **forma de *ser*** em um verbo passivo é tipicamente uma das seguintes palavras:
  * é/são
  * foi/foram
* Um verbo de **particípio passado** é tipicamente um verbo na sua forma passada e é nominal, ou seja, tem o papel de substituir um nome. Por exemplo, os seguintes são verbos de particípio passado:
  * interpretado
  * gerado
  * formado

Colocar a forma de *ser* e o particípio passado juntos produz verbos passivos, como o seguinte:

* foi interpretado
* é gerado
* foi formado
* é congelado

Se a frase contém um ator, uma preposição geralmente segue o verbo passivo. (Essa preposição costuma ser uma pista importante para ajudá-lo a identificar a voz passiva.) Os exemplos a seguir combinam o verbo passivo e a preposição:

* foi interpretado como
* é gerado por
* foi formado por
* é congelado por

### Os verbos imperativos são tipicamente ativos

É fácil classificar erroneamente frases que começam com um **verbo imperativo** como passivas. Um verbo imperativo é um comando. Muitos itens em listas numeradas começam com verbos imperativos. Por exemplo, *Abra* e *Defina* na lista a seguir são verbos imperativos:

1. Abra o arquivo de configuração.
2. Defina a variável `Frombus` como `False`.

As sentenças que começam com um verbo no imperativo geralmente estão na voz ativa, embora não mencionem explicitamente um ator. Em vez disso, o ator fica *implícito* nas frases que começam com um verbo imperativo. O ator implícito é **você**.

### Exercício

Marque cada uma das seguintes frases como **Passiva** ou **Ativa**:

1. O `MutableInput` fornece acesso somente como leitura.
2. O acesso somente como leitura é fornecido pelo `MutableInput`.
3. O desempenho foi medido.
4. Python foi inventado por Guido van Rossum no século XX.
5. David Korn descobriu o KornShell por acaso.
6. Essas informações são usadas pela equipe de aplicação de políticas.
7. Clique no botão Enviar.
8. A órbita foi calculada por Katherine Johnson.

<details>
<summary>Clique para revelar a resposta.</summary>

<ol>
  <li><b>Ativa</b>. O <code>MutableInput</code> fornece acesso somente leitura.</li>
  <li><b>Passiva</b>. O acesso somente como leitura é fornecido pelo <code>MutableInput</code>.</li>
  <li><b>Passiva</b>. O desempenho foi medido.</li>
  <li><b>Passiva</b>. Python foi inventado por Guido van Rossum no século XX.</li>
  <li><b>Ativa</b>. David Korn descobriu o KornShell por acaso.</li>
  <li><b>Passiva</b>. Essas informações são usadas pela equipe de aplicação de políticas.</li>
  <li><b>Ativa</b>. Clique no botão Enviar. (<i>Clique</i> é um verbo imperativo.)</li>
  <li><b>Passiva</b>. A órbita foi calculada por Katherine Johnson.</li>
</ol>

</details>

## Distinguir a voz ativa da voz passiva em frases mais complexas

Muitas frases contêm vários verbos, onde alguns são ativos e alguns são passivos. Por exemplo, a frase a seguir contém dois verbos na voz passiva:

![O código [alvo] é interpretado [verbo passivo] em Python [ator], mas o código [alvo] é compilado [verbo passivo] em C++ [ator].](/res/img/curso/passiva-passiva.png "O código [alvo] é interpretado [verbo passivo] em Python [ator], mas o código [alvo] é compilado [verbo passivo] em C++ [ator].")

Aqui está a mesma frase, parcialmente convertida em voz ativa:

![Python [ator] interpreta [verbo ativo] o código [alvo], mas o código [alvo] é compilado [verbo passivo] em C++ [ator].](/res/img/curso/ativa-passiva.png "Python [ator] interpreta [verbo ativo] o código [alvo], mas o código [alvo] é compilado [verbo passivo] em C++ [ator].")

E aqui está a mesma frase, agora totalmente convertida em voz ativa:

![Python [ator] interpreta [verbo ativo] o código [alvo], mas C++ [ator] compila [verbo ativo] o código [alvo].](/res/img/curso/ativa-ativa.png "Python [ator] interpreta [verbo ativo] o código [alvo], mas C++ [ator] compila [verbo ativo] o código [alvo].")

### Exercício

Cada uma das frases a seguir contém dois verbos. Classifique cada um dos verbos nas frases a seguir como ativo ou passivo. Por exemplo, se o primeiro verbo for ativo e o segundo for passivo, escreva **Ativo**, **Passivo**.

1. A equipe de controle de qualidade adora picolé, mas os redatores preferem sorvete.
2. As métricas de desempenho são exigidas pela equipe, embora eu prefira palpites malucos.
3. Quando engenheiras de software tentam algo novo e inovador, uma recompensa deve ser dada.

<details>
<summary>Clique para revelar a resposta.</summary>

<ol>
  <li><b>Ativo, Ativo</b>. equipe de controle de qualidade adora picolé, mas os redatores preferem sorvete.</li>
  <li><b>Passivo, Ativo</b>. As métricas de desempenho são exigidas pela equipe, embora eu prefira palpites malucos.</li>
  <li><b>Ativo, Passivo</b>. Quando engenheiras de software tentam algo novo e inovador, uma recompensa deve ser dada.</li>
</ol>

</details>

## Prefira a voz ativa à voz passiva

Use a voz ativa na maioria das vezes. Use a voz passiva com moderação. A voz ativa oferece as seguintes vantagens:

* A maioria dos leitores converte mentalmente a voz passiva em voz ativa. Por que sujeitar seus leitores a um tempo extra de processamento? Aderindo à voz ativa, os leitores podem pular o estágio do pré-processador e ir direto para a compilação.
* A voz passiva ofusca suas ideias, virando frases de cabeça para baixo. A voz passiva relata a ação indiretamente.
* Algumas frases de voz passiva omitem completamente um ator, o que força o leitor a adivinhar a identidade do ator.
* A voz ativa é geralmente mais curta que a voz passiva.

### Relatórios de pesquisa científica (material opcional)

A voz passiva corre solta em certos relatórios de pesquisas científicas. Nesses relatórios de pesquisa, os pesquisadores e métodos que foram usados geralmente somem, levando a frases passivas que começam assim:

* Foi sugerido que...
* Os dados foram tirados...
* As estatísticas foram calculadas...
* Os resultados foram avaliados.

Sabemos quem está fazendo o que a quem? Não. A voz passiva de alguma forma torna a informação mais objetiva? Não.

Muitas revistas científicas adotaram a voz ativa. Encorajamos o resto das pessoas a se juntar à busca por clareza.

### Exercício

Reescreva as seguintes frases de voz passiva como voz ativa. Apenas parte de algumas frases estão na voz passiva; garanta que todas as partes terminem como voz ativa:

1. As bandeiras não foram analisadas pelo Mungifier.
2. Um wrapper é gerado pelo processo de registro de Op.
3. Apenas um experimento por camada é selecionado pelo sistema Frombus.
4. As métricas de qualidade são identificadas por asteriscos; o negrito identifica métricas ruins.

<details>
<summary>Clique para revelar a resposta.</summary>

<ol>
  <li>O Mungifier não analisou as bandeiras.</li>
  <li>O processo de registro de Op gera um wrapper.</li>
  <li>O sistema Frombus seleciona apenas um experimento por camada.</li>
  <li>Asteriscos identificam métricas de qualidade; o negrito identifica métricas ruins.</li>
</ol>

</details>

---

<p class="proxima-unidade"><b>Próxima unidade:</b> <a href="/curso/modulo-1/frases-claras/"><button type="button" class="btn btn-dark">Frases claras</button></a></p>

[^1]: "Dar o pontapé inicial" é uma expressão idiomática que significa "começar algo".

{% include footer-conteudo-traduzido.html %}
