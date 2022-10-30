---
layout: curso-modulo-1
title: Palavras
permalink: /curso/modulo-1/palavras/
---

# Palavras

<div class="alerta alerta-simples">
    <p>Tempo estimado: 10 minutos</p>
</div>

Nós pesquisamos documentações extensivamente, e acontece que as melhores frases do mundo consistem principalmente de palavras. (*Sarcasmo...*)

## Defina termos novos ou desconhecidos

Ao escrever ou editar, aprenda a reconhecer termos que podem ser desconhecidos para alguns ou todos os seus públicos-alvo. Ao identificar esse termo, adote uma das duas táticas a seguir:

* Se o termo já existir, vincule a uma boa explicação existente. (Não reinvente a roda.)
* Se o seu documento estiver introduzindo o termo pela primeira vez, defina o termo. Se o seu documento estiver introduzindo muitos termos, reúna as definições em um glossário.

## Use termos de forma consistente

Se você alterar o nome de uma variável no meio de um método, seu código não será compilado. Da mesma forma, se você renomear um termo no meio de um documento, suas ideias não serão compiladas (na cabeça de seus usuários).

A moral: aplique a mesma palavra ou termo sem ambiguidade e de forma consistente em todo o seu documento. Depois de nomear um componente **coisa**, não o renomeie como **treco**. Por exemplo, o parágrafo a seguir renomeia erroneamente **Buffers de Protocolo** para **protobufs**:

> Os Buffers de Protocolo têm sua própria linguagem de definição. Blá blá blá. E é por isso que os protobufs venceram tantas feiras municipais.

George Fairbanks, um engenheiro de software do Google, fez esta excelente observação sobre nomenclatura consistente:

> Quando encontro duas palavras que parecem ser sinônimos, me pergunto se o autor está tentando sinalizar uma distinção sutil que preciso buscar e entender.

Sim, a redação técnica é cruel e restritiva, mas pelo menos a redação técnica oferece uma excelente solução alternativa. Ou seja, ao introduzir um nome de conceito ou nome de produto prolixo, você também pode especificar uma versão abreviada desse nome. Em seguida, você pode usar esse nome abreviado em todo o documento. Por exemplo, o parágrafo a seguir está bom:

> **Buffers de Protocolo** (ou **protobufs** para abreviar) têm sua própria linguagem de definição. Blá blá blá. E é por isso que os protobufs venceram tantas feiras municipais.

## Use siglas corretamente

No uso inicial de uma sigla desconhecida em um documento ou seção, descreva o termo completo e, em seguida, coloque a sigla entre parênteses. Coloque a versão por extenso e a sigla em negrito. Por exemplo:

> Este documento é para engenheiros que são novos na **Rede Tátil Telecinética** (**TTN**) ou precisam entender como solicitar peças de reposição TTN por meio de movimentos dos dedos.

Você pode então usar a sigla daqui para frente, como no exemplo a seguir:

> Se não existir nenhuma entrada de cache, o Mixer chama o **OttoGroup Server** (**OGS**) para buscar Ottos para a solicitação. O OGS é um repositório que contém todos os Ottos servíveis. O OGS está organizado em uma estrutura de árvore lógica, com um nó raiz e dois níveis de nós derivados. A raiz OGS encaminha a solicitação para as derivações e coleta as respostas.

Não alterne entre a sigla e a versão por extenso no mesmo documento.

### Usar a sigla ou o termo completo?

Claro, você pode introduzir e usar siglas do jeito certo, mas você *deve* usar siglas? Bem, siglas reduzem o tamanho da frase. Por exemplo, *TTN* é duas palavras mais curta do que *Rede Tátil Telecinética*. No entanto, siglas são realmente apenas uma camada de abstração; os leitores devem expandir mentalmente as siglas recém aprendidas para o termo completo. Por exemplo, os leitores convertem *TTN* para *Rede Tátil Telecinética* em suas cabeças, então a sigla "mais curta" na verdade demora um pouco mais para ser processada do que o termo completo.

Siglas muito usadas ​criam a sua própria identidade. Após várias ocorrências, os leitores geralmente param de expandir as siglas para o termo completo. Muitos desenvolvedores da Web, por exemplo, esqueceram qual é a versão por extenso de *HTML*.

Aqui estão as diretrizes para siglas:

* Não estabeleça siglas que seriam usadas poucas vezes.
* Estabeleça siglas que atendam a ambos os critérios a seguir:
  * A sigla é significativamente mais curta do que o termo completo.
  * A sigla aparece muitas vezes no documento.

### Exercício

Corrija a seguinte passagem. Suponha que esta passagem seja a primeira menção ao termo **MapReduce** no documento e que **MR** seja a melhor abreviação.

> Jeff Dean inventou o MapReduce em 1693, implementando o algoritmo em um computador baseado em silício fabricado com areia de praia, papel encerado, uma caneta e uma torradeira. Esta versão do MR bateu vários recordes mundiais de desempenho até 2014.

(Observe que a passagem anterior pretende ser humorística, não factual.)

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Você pode tomar algumas abordagens diferentes aqui. Uma abordagem é associar a sigla <i>MR</i> ao termo completo e depois usar essa sigla:</p>

<blockquote>Jeff Dean inventou o <b>MapReduce</b> (<b>MR</b>) em... Esta versão do MR bateu vários...</blockquote>

<p>Alternativamente, você pode decidir que abreviar uma passagem tão curta sobrecarrega muito os leitores, então você simplesmente usará o termo <i>MapReduce</i> completo todas as vezes:</p>

<blockquote>Jeff Dean inventou o <b>MapReduce</b> em... Esta versão do MapReduce bateu vários...</blockquote>

<p>Aliás, um redator técnico mais experiente também converteria "areia de praia, papel encerado, uma caneta e uma torradeira" em uma lista com marcadores. Você aprenderá mais sobre isso na <a href="/curso/modulo-1/listas-tabelas/">lição de Listas e Tabelas</a>.</p>

</details>

## Identifique os pronomes ambíguos

Muitos pronomes apontam para um substantivo previamente mencionado. Assim como acontece com ponteiros na programação, os pronomes tendem a causar alguns erros. Usar pronomes incorretamente causa o equivalente a um erro de ponteiro nulo (*null pointer*) na cabeça de seus leitores. Em muitos casos, você deve simplesmente evitar o pronome e reutilizar o substantivo. No entanto, a utilidade de um pronome às vezes supera seu risco (como nesta frase).

Considere as seguintes diretrizes de pronome:

* Só use um pronome *depois* de introduzir o substantivo; nunca use o pronome antes de introduzir o substantivo.
* Coloque o pronome o mais próximo possível do substantivo referente. Geralmente, se mais de cinco palavras separam o substantivo do pronome, é melhor repetir o substantivo em vez de usar o pronome.
* Se você introduzir um segundo substantivo entre seu substantivo e seu pronome, reutilize seu substantivo em vez de usar um pronome.

### Isto e ele

Os seguintes pronomes causam mais confusão na documentação técnica:

* isto
* ele(s), seu(s) e dele(s)

Por exemplo, na frase a seguir, **Ele** se refere a Python ou a C++?

> Python é interpretado, enquanto C++ é compilado. **Ele** tem um seguimento que é quase *cult*.

Como outro exemplo, a que se refere a palavra **seu** na frase a seguir?

> Tenha cuidado ao usar Frambus ou Carambola com HoobyScooby ou BoiseFram, porque um bug em **seu** núcleo pode causar desamizamento em massa acidental.

### Isso e aquilo

Considere os seguintes pronomes também como problemáticos:

* isso
* aquilo

Por exemplo, na frase ambígua a seguir, **Isso** pode se referir ao ID do usuário, à execução do processo ou a todos eles:

> A execução do processo configura permissões e gera um ID do usuário. **Isso** permite que os usuários se autentiquem no aplicativo.

Para ajudar os leitores, evite usar **isso** ou **aquilo** de forma que não esteja claro a que se referem. Use uma das seguintes táticas para esclarecer usos ambíguos de **isso** e **aquilo**:

* Substitua **isso** ou **aquilo** pelo substantivo apropriado.
* Coloque um substantivo imediatamente após **isso** ou **aquilo**.

Substitua ou adicione termos explícitos conforme necessário, como nas seguintes reescritas da segunda frase do exemplo:

> Esse ID de usuário permite que os usuários se autentiquem.
>
> O processo de configuração de permissões permite que os usuários se autentiquem.
>
> A combinação de permissões e um ID de usuário permite que os usuários se autentiquem.

### Exercício

Identifique todos os significados possíveis para os pronomes ambíguos em cada uma das seguintes passagens:

1. Amanda e Felipe compartilham responsabilidades com Maísa e Carlos. Eles são os próximos de plantão.

2. Você pode importar os dados do Carambola através do seu arquivo de configuração ou dinamicamente em tempo de execução. Isso pode ser um risco de segurança.

<details>
<summary>Clique para revelar a resposta.</summary>

<ol>
  <li>O pronome <b>eles</b> poderia se referir a qualquer um dos seguintes:
    <ul>
      <li>Amanda e Felipe</li>
      <li>Maísa e Carlos</li>
      <li>Amanda, Felipe, Maísa e Carlos</li>
    </ul>
  </li>
  <li>O pronome <b>isso</b> pode se referir a qualquer um dos seguintes:
    <ul>
      <li>importar através do arquivo de configuração</li>
      <li>importar dinamicamente em tempo de execução</li>
      <li>ambas</li>
    </ul>
  </li>
</ol>

</details>

---

<p class="proxima-unidade"><b>Próxima unidade:</b> <a href="/curso/modulo-1/voz-ativa/"><button type="button" class="btn btn-dark">Voz ativa vs. voz passiva</button></a></p>

{% include footer-conteudo-traduzido.html %}
