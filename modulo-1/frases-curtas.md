---
layout: curso-modulo-1
title: Frases curtas
permalink: /curso/modulo-1/frases-curtas/
---

# Frases curtas

<div class="alerta alerta-simples">
    <p>Tempo estimado: 20 minutos</p>
</div>

Engenheiros de software geralmente tentam minimizar o número de linhas de código em uma implementação pelos seguintes motivos:

* Código mais curto é normalmente mais fácil para outros lerem.
* Código mais curto é normalmente mais fácil de manter do que código mais longo.
* Linhas extras de código introduzem pontos adicionais de falha.

De fato, as mesmas regras se aplicam à redação técnica:

* Documentação mais curta é mais rápida de ler do que documentação mais longa.
* Documentação mais curta é normalmente mais fácil de manter do que documentação mais longa.
* Linhas extras de documentação introduzem pontos adicionais de falha.

Implementar uma documentação mais curta leva tempo, mas vale a pena. Frases curtas se comunicam melhor do que frases longas, e frases curtas geralmente são mais fáceis de entender do que frases longas.

## Concentre uma única ideia em cada frase

Concentre cada frase em uma única ideia, pensamento ou conceito. Assim como as instruções em um programa executam uma única tarefa, as sentenças devem executar uma única ideia. Por exemplo, a frase muito longa a seguir contém vários pensamentos:

> O final da década de 1950 foi uma era chave para as linguagens de programação, porque a IBM introduziu o Fortran em 1957 e John McCarthy introduziu o Lisp no ano seguinte, o que deu aos programadores uma maneira iterativa de resolver problemas e uma maneira recursiva.

Quebrar a frase longa em uma sucessão de frases de ideia única produz o seguinte resultado:

> O final da década de 1950 foi uma era chave para as linguagens de programação. A IBM introduziu o Fortran em 1957. John McCarthy inventou o Lisp no ano seguinte. Consequentemente, no final da década de 1950, os programadores podiam resolver problemas de forma iterativa ou recursiva.

### Exercício

Converta a seguinte frase excessivamente longa em uma série de frases mais curtas. Não revise muito; apenas termine com algumas frases em vez de apenas uma.

> No bash, use as instruções if, then e fi para implementar um bloco de ramificação condicional simples no qual a instrução if avalia uma expressão, a instrução then introduz um bloco de instruções a serem executadas quando a expressão if for verdadeira e a instrução fi marca o final do bloco de ramificação condicional.

<details>
<summary>Clique para revelar a resposta.</summary>

<p>No bash, use uma instrução if, then e fi para implementar um bloco de ramificação condicional simples. A instrução if avalia uma expressão. A instrução then introduz um bloco de instruções a serem executadas quando a expressão if for verdadeira. A instrução fi marca o fim do bloco de ramificação condicional. <i>(O parágrafo resultante continua não sendo claro, mas ainda é muito mais fácil de ler do que a frase original.)</i></p>

</details>

## Converta algumas frases longas em listas

Dentro de muitas frases técnicas longas há uma lista querendo se libertar. Por exemplo, considere a seguinte frase:

> Para alterar o fluxo normal de um loop, você pode usar uma instrução `break` (que o pula para fora do loop atual) ou uma instrução `continue` (que pula o restante da iteração atual do loop atual).

Quando você vir a conjunção **ou** em uma frase longa, considere refatorar essa frase em uma lista com marcadores. Quando você vir uma lista de itens ou tarefas incorporada em uma frase longa, considere refatorar essa frase em uma lista com marcadores ou numerada. Por exemplo, o exemplo anterior contém a conjunção **ou**, então vamos converter essa frase longa para a seguinte lista com marcadores:

> Para alterar o fluxo normal de um loop, chame uma das seguintes instruções:
>
> * `break`, que faz você sair do loop atual.
> * `continue`, que pula o restante da iteração atual do loop atual.

### Exercício

Refatore as frases a seguir em algo mais curto e claro. Certifique-se de que sua resposta contém uma lista:

1. Para começar a usar o aplicativo Frambus, você deve primeiro encontrar o aplicativo em uma loja adequada, comprá-lo usando um cartão de crédito ou débito válido, baixá-lo, configurá-lo atribuindo um valor para a variável `Foo` no arquivo `/etc/Frambus` e, em seguida, execute-o falando a palavra mágica duas vezes.
2. KornShell foi inventado por David Korn em 1983, um cientista da computação da Bell Labs na época, como um superconjunto de recursos, aprimoramentos e melhorias sobre o Bourne Shell (com o qual era compatível em versões anteriores), que foi inventado por Stephen Bourne em 1977, que foi também cientista da computação no Bell Labs.

<details>
<summary>Clique para revelar a resposta.</summary>

<p><b>Frase 1</b></p>

<p>Siga os seguintes passos para começar a usar o aplicativo Frambus:</p>

<ol>
    <li>Encontre o aplicativo em uma loja adequada.</li>
    <li>Compre o aplicativo usando um cartão de crédito ou débito válido.</li>
    <li>Baixe o aplicativo.</li>
    <li>Configure o aplicativo atribuindo um valor para a variável <code>Foo</code> no arquivo <code>/etc/Frambus</code>.</li>
    <li>Execute o aplicativo falando a palavra mágica duas vezes.</li>
</ol>

<p><b>Frase 2</b></p>

<p>Os seguintes dois cientistas da computação do Bell Labs inventaram shells populares:</p>

<ul>
    <li>Stephen Bourne inventou o Bourne Shell em 1977.</li>
    <li>David Korn inventou o KornShell em 1983.</li>
</ul>

<p>O KornShell é um superconjunto compatível com versões anteriores do Bourne Shell, contendo muitas melhorias em relação ao shell mais antigo.</p>

</details>

## Elimine ou reduza palavras desnecessárias

Muitas frases contêm palavras que apenas incham o texto — lixo textual que consome espaço sem ajudar o leitor. Por exemplo, veja se você consegue identificar as palavras desnecessárias na seguinte frase:

> Um valor de entrada maior que 100 causa o acionamento do log.

Substituir **causa o acionamento do** com o verbo mais curto **aciona** resulta numa frase mais curta:

> Um valor de entrada maior que 100 aciona o log.

Com a prática, você identificará as palavras extras e ficará muito feliz em removê-las ou reduzi-las. Por exemplo, considere a seguinte frase:

> Este documento de design fornece uma descrição detalhada do Projeto Frambus.

A frase **fornece uma descrição detalhada de** se reduz ao verbo **descreve** (ou o verbo **detalha**), de modo que a sentença resultante pode se tornar:

> Este documento de design descreve o Projeto Frambus.

A tabela a seguir sugere substituições para algumas frases que normalmente podem ser reduzidas:

<table class="table">
    <thead class="table-light">
        <tr>
            <th>Palavras demais</th>
            <th>Conciso</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>no momento atual</td>
            <td>agora</td>
        </tr>
        <tr>
            <td>determinar a localização de</td>
            <td>encontrar</td>
        </tr>
        <tr>
            <td>é capaz de</td>
            <td>pode</td>
        </tr>
    </tbody>
</table>

### Exercício

Encurte as seguintes frases sem alterar o seu significado:

1. Apesar do fato de Arnaldo escrever código com bugs, ele escreve documentação livre de erros.
2. A mudança da frase da voz passiva para a voz ativa aumenta o esclarecimento dos pontos-chave.
3. Descubra se Roberta é capaz de escrever código em COBOL.
4. O Frambus causa a produção de bugs, que serão registrados em logs pelo método LogGenerator.

<details>
<summary>Clique para revelar a resposta.</summary>

<p><b>Aqui estão algumas soluções possíveis:</b></p>

<ol>
    <li>Embora Arnaldo escreva código com bugs, ele escreve documentação sem erros.
        <ul>
            <li><b>Resposta alternativa:</b> Arnaldo escreve código com bugs. No entanto, ele escreve documentação livre de erros.</li>
        </ul>
    </li>
    <li>Mudar a frase da voz passiva para a voz ativa esclarece os pontos-chave.</li>
    <li>Descubra se Roberta sabe codificar em COBOL.</li>
    <li>O Frambus produz bugs, os quais o método LogGenerator registra.</li>
</ol>

</details>

## Reduza orações subordinadas (opcional)

Uma sentença é um fragmento lógico independente de uma oração, a qual contém um ator e uma ação. Cada sentença contém o seguinte:

* uma oração principal
* zero ou mais orações subordinadas

As orações subordinadas modificam a ideia da oração principal. Como o nome indica, as orações subordinadas são menos importantes que a oração principal. Por exemplo, considere a seguinte frase:

> Python é uma linguagem de programação interpretada, que foi inventada em 1991.
>
> * cláusula principal: Python é uma linguagem de programação interpretada
> * oração subordinada: que foi inventada em 1991

Geralmente você pode identificar orações subordinadas pelas palavras que as introduzem. A lista a seguir (longe de estar completa) mostra palavras comuns que introduzem orações subordinadas:

* que
* o(a) qual
* porque
* do(a) qual
* até
* a menos que
* desde

Algumas orações subordinadas começam com uma vírgula e outras não. A oração subordinada destacada na frase a seguir, por exemplo, começa com a palavra **porque** e não contém vírgula:

<blockquote>Prefiro codificar em C++ <span class="highlight-azul">porque gosto de tipagem de dados forte.</span></blockquote>

Ao editar um texto, avalie as orações subordinadas. Siga o conceito de `uma frase = uma ideia em mente`. As orações subordinadas de uma frase ampliam a ideia principal ou se ramificam em uma nova ideia separada? Se for a segunda opção, considere dividir a(s) oração(ões) subordinada(s) ofensora(s) em frases separadas.

### Exercício

Determine quais das frases contêm orações subordinadas que devem ser ramificadas em frases separadas. (Não reescreva as frases, apenas identifique as frases que devem ser reescritas.)

1. Python é uma linguagem interpretada, o que significa que a linguagem pode executar o código-fonte diretamente.
2. Bash é uma linguagem de script shell moderna que busca muitos de seus recursos do KornShell 88, que foi desenvolvido no Bell Labs.
3. Lisp é uma linguagem de programação que se baseia na notação de prefixo polonês, que é um dos sistemas inventados pelo lógico polonês Jan Łukasiewicz.
4. Não quero dizer que o Fortran é antigo, mas apenas a datação por radiocarbono pode determinar sua verdadeira idade.

<details>
<summary>Clique para revelar a resposta.</summary>

<p>As orações subordinadas estão sombreadas a seguir:</p>

<ol>
    <li>Python é uma linguagem interpretada, <span class="highlight-azul">o que significa que a linguagem pode executar o código-fonte diretamente.</span>
        <ul>
            <li><b>A oração subordinada nesta frase estende a ideia principal, então esta frase está boa.</b></li>
        </ul>
    </li>
    <li>Bash é uma linguagem de script shell moderna <span class="highlight-azul">que busca muitos de seus recursos do KornShell 88,</span><span class="highlight-amarelo"> que foi desenvolvido no Bell Labs.</span>
        <ul>
            <li><b>A primeira oração subordinada amplia a ideia principal, mas a segunda oração subordinada leva para outra direção. Divida esta frase em duas.</b></li>
        </ul>
    </li>
    <li>Lisp é uma linguagem de programação <span class="highlight-azul">que se baseia na notação de prefixo polonês,</span><span class="highlight-amarelo"> que é um dos sistemas inventados pelo lógico polonês Jan Łukasiewicz.</span>
        <ul>
            <li><b>A primeira oração subordinada é claramente crítica para a sentença, mas a segunda oração subordinada leva o leitor muito longe da oração principal. Divida esta frase em duas.</b></li>
        </ul>
    </li>
    <li>Não quero dizer que o Fortran é antigo, <span class="highlight-azul">mas apenas a datação por radiocarbono pode determinar sua verdadeira idade.</span>
        <ul>
            <li><b>A oração subordinada é fundamental para a frase, então esta frase está boa.</b></li>
        </ul>
    </li>
</ol>

</details>

## Diferencie "que" de "o(a) qual"

**Que** e **o(a) qual** quase sempre iniciam orações subordinadas. Qual é a diferença entre eles? Bem, no Brasil, ambos são praticamente intercambiáveis.

No entanto, procure reservar **o(a) qual** para orações subordinadas não essenciais e usar **que** para uma oração subordinada essencial sem a qual a sentença não pode viver. Por exemplo, a mensagem principal na frase a seguir é que Python é uma linguagem interpretada; a frase pode sobreviver sem Guido van Rossum ser o inventor:

> Python é uma linguagem interpretada, **a qual** Guido van Rossum inventou.

Por outro lado, a seguinte frase precisa do trecho **que não envolvem álgebra linear**:

> Fortran é perfeito para cálculos matemáticos **que** não envolvem álgebra linear.

Se você ler uma frase em voz alta e perceber uma pausa antes da oração subordinada, use **o(a) qual**. Se você não perceber uma pausa, use **que**. Volte e leia as duas frases de exemplo anteriores. Você ouve a pausa na primeira frase?

Coloque uma vírgula antes de **o(a) qual**; não coloque uma vírgula antes de **que**.

---

<p class="proxima-unidade"><b>Próxima unidade:</b> <a href="/curso/modulo-1/listas-tabelas/"><button type="button" class="btn btn-dark">Listas e tabelas</button></a></p>

{% include footer-conteudo-traduzido.html %}
