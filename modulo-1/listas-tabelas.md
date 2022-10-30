---
layout: curso-modulo-1
title: Listas e tabelas
permalink: /curso/modulo-1/listas-tabelas/
---

# Listas e tabelas

<div class="alerta alerta-simples">
    <p>Tempo estimado: 15 minutos</p>
</div>

Boas listas podem transformar o caos técnico em algo ordenado. Leitores técnicos geralmente adoram listas. Portanto, ao escrever, identifique as oportunidades de converter informações em listas.

## Escolha o tipo correto de lista

Os seguintes tipos de listas são comuns na redação técnica:

* listas com marcadores
* listas numeradas
* listas incorporadas

Use uma lista com marcadores (•) para itens não ordenados; use uma lista numerada (1, 2, 3, ...) para itens ordenados. Em outras palavras:

* Se você reorganizar os itens em uma lista com marcadores, o significado da lista não será alterado.
* Se você reorganizar os itens em uma lista numerada, o significado da lista muda.

Por exemplo, a lista seguinte usa marcadores porque reorganizar seus itens não altera o significado da lista:

> O Bash fornece os seguintes mecanismos de manipulação de strings:
>
> * excluindo uma substring do início de uma string
> * lendo um arquivo inteiro em uma variável de string

A lista a seguir, por outro lado, deve ser uma lista numerada porque reorganizar seus itens mudaria o significado da lista:

> Execute as seguintes etapas para reconfigurar o servidor:
>
> 1. Pare o servidor.
> 2. Edite o arquivo de configuração.
> 3. Reinicie o servidor.

Uma **lista incorporada** (às vezes chamada de **lista em texto corrido**) contém itens embutidos em uma frase. Por exemplo, a frase a seguir contém uma lista incorporada com quatro itens:

> A API `capturalhamas` permite que as chamadas criem e consultem lhamas, analisem alpacas, excluam vicunhas e rastreiem dromedários.

De um modo geral, as listas incorporadas são uma maneira ruim de apresentar informações técnicas. Tente transformar listas incorporadas em listas com marcadores ou listas numeradas. Por exemplo, você deve converter a frase do exemplo anterior na seguinte passagem:

> A API `capturalhamas` permite que as chamadas façam o seguinte:
>
> * Criar e consultar lhamas.
> * Analisar as alpacas.
> * Excluir vicunhas.
> * Rastrear dromedários.

### Exercício

Converta o seguinte parágrafo em uma ou mais listas:

> Hoje no trabalho, tenho que codificar três testes unitários, escrever uma documentação de projeto e revisar a documentação da Janete. Depois do trabalho, tenho que lavar meu carro sem usar água e depois secá-lo sem usar toalhas.

Não se esqueça de dar uma introdução para a(s) sua(s) lista(s).

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Aqui está uma possível resposta:</p>

<blockquote>

<p>Devo fazer o seguinte no trabalho hoje:</p>

<ul>
    <li>Codificar três testes unitários.</li>
    <li>Escrever uma documentação de projeto.</li>
    <li>Revisar a documentação da Janete.</li>
</ul>

<p>Depois do trabalho, devo fazer o seguinte</p>

<ol>
    <li>Lavar meu carro sem usar água.</li>
    <li>Secar meu carro sem usar toalhas.</li>
</ol>

</blockquote>

<p>Segue uma resposta alternativa:</p>

<blockquote>

<p>Devo fazer as seguintes tarefas hoje:</p>

<ul>
    <li>No trabalho:
        <ul>
            <li>Codificar três testes unitários.</li>
            <li>Escrever uma documentação de projeto.</li>
            <li>Revisar a documentação da Janete.</li>
        </ul>
    </li>
    <li>Depois do trabalho:
        <ol>
            <li>Lavar meu carro sem usar água.</li>
            <li>Secar meu carro sem usar toalhas.</li>
        </ol>
    </li>
</ul>

</blockquote>

</details>

## Mantenha os itens da lista simétricos

O que separa as listas eficazes das problemáticas? Listas eficazes são **simétricas**; listas problemáticas tendem a ser assimétricas. Todos os itens em uma lista simétricas parecem "pertencer" um ao outro. Ou seja, todos os itens em uma lista simétrica atendem aos seguintes critérios:

* gramática
* categoria lógica
* capitalização de texto
* pontuação

Por outro lado, pelo menos um item em uma lista **assimétrica** falha em pelo menos um dos requisitos acima.

Por exemplo, a lista a seguir é simétrica porque todos os itens são substantivos no plural (gramática), comestíveis (categoria lógica), letras minúsculas (capitalização) e sem pontos ou vírgulas (pontuação).

* cenouras
* batatas
* repolhos

Por outro lado, a lista a seguir é dolorosamente assimétrica em todos os quatro parâmetros:

* cenouras
* batatas
* A luz do verão obscurece todas as lembranças do inverno.

A lista a seguir é simétrica porque todos os itens são frases completas com letras maiúsculas e pontuação completas:

* As cenouras contêm muita vitamina A.
* As batatas ficaram deliciosas.
* Os repolhos fornecem grande quantidade de vitamina K.

O primeiro item de uma lista estabelece um padrão que os leitores esperam ver repetidos nos itens subsequentes.

### Exercício

A lista a seguir é simétrica ou assimétrica?

* Brócolis inspira sentimentos de amor ou ódio.
* As batatas ficaram deliciosas.
* Repolhos.

<details>
<summary>Clique para revelar a resposta.</summary>

<p>A lista não é simétrica. Os dois primeiros itens são frases completas, mas o terceiro item não é uma frase. (Não se deixe enganar pela capitalização e pontuação do terceiro item.)</p>

</details>

### Exercício

A lista a seguir é simétrica ou assimétrica?

* Os pontos vermelhos representam árvores doentes.
* As árvores imaturas são representadas pelos pontos azuis.
* Os pontos verdes representam árvores saudáveis.

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Esta lista não é simétrica. O primeiro e terceiro itens estão na voz ativa, mas o segundo item está na voz passiva.</p>

</details>

## Inicie itens de lista numerada com verbos imperativos

Considere iniciar todos os itens em uma lista numerada com um **verbo imperativo**. Um verbo imperativo é um comando, como **abrir** ou **iniciar**. Por exemplo, observe como todos os itens na lista numerada simétrica a seguir começam com um verbo imperativo:

1. Baixe o aplicativo Frambus no Google Play ou iTunes.
2. Defina as configurações do aplicativo Frambus.
3. Inicie o aplicativo Frambus.

A lista numerada a seguir não é simétrica porque duas das frases começam com um verbo imperativo, mas o terceiro item não:

1. Instancie a classe Froobus.
2. Invoque o método `Froobus.Salmonella()`.
3. O processo para.

### Exercício

Faça com que a seguinte lista fique simétrica. Certifique-se de que cada elemento na lista resultante comece com um verbo imperativo:

1. Pare o Frambus
2. O arquivo de configuração de chave é `/etc/frambus`. Abra este arquivo com um editor de texto ASCII.
3. Neste arquivo, você verá um parâmetro chamado `Carambola`, que atualmente está definido com o valor padrão (32). Altere este valor para 64.
4. Quando terminar de definir este parâmetro, salve e feche o arquivo de configuração
5. agora, inicie o Frambus novamente.

<details>
<summary>Clique para revelar a resposta.</summary>

<p>A seguir, uma resposta possível:</p>

<ol>
    <li>Pare o Frambus.</li>
    <li>Abra o arquivo de configuração de chave, <code>/etc/frambus</code>, com um editor de texto ASCII.</li>
    <li>Altere o parâmetro <code>Carambola</code> de seu valor padrão (32) para 64.</li>
    <li>Salve e feche o arquivo de configuração.</li>
    <li>Reinicie o Frambus.</li>
</ol>

</details>

## Aplique a pontuação adequada aos itens

Se o item da lista for uma frase, inicie com letras maiúsculas e termine com pontuação. Caso contrário, não use letras maiúsculas e pontuação. Por exemplo, o item da lista a seguir é uma frase, então colocamos o **M** maiúsculo em **Muitas** e colocamos um ponto no final da frase:

* Muitas carambolas têm cinco cristas.

No entanto, o item da lista a seguir não é uma sentença completa, então deixamos o **c** em minúsculo e omitimos um ponto final:

* cor dos limões

## Crie tabelas úteis

Mentes analíticas costumam amar tabelas. Quando uma página apresenta vários parágrafos e uma única tabela, os olhos de leitores técnicos se dirigem para a tabela.

Considere as seguintes diretrizes ao criar tabelas:

* Rotule cada coluna com um cabeçalho significativo. Não faça os leitores adivinharem o que cada coluna contém.
* Evite colocar muito texto em uma célula da tabela. Se uma célula da tabela contém mais de duas frases, pergunte a si mesmo se essa informação deveria ter outro formato.
* Embora colunas diferentes possam conter diferentes tipos de dados, esforce-se pela semelhança do conteúdo **dentro** de cada coluna. Por exemplo, as células dentro de uma mesma coluna da tabela não devem ser uma mistura de dados numéricos e nomes de artistas famosos.

<div class="alerta alerta-azul">
    <p>Algumas tabelas não ficam bem formatadas em todos os tamanhos de tela. Por exemplo, uma tabela que fica boa no seu laptop pode ficar horrível no seu telefone.</p>
</div>

## Dê uma introução para cada lista e tabela

Recomendamos fazer uma introdução para cada lista e tabela, com uma frase que diga aos leitores o que a lista ou tabela representa. Em outras palavras, dê o contexto da lista ou da tabela. Termine a frase introdutória com dois pontos em vez de um ponto.

Embora não seja um requisito, recomendamos incluir a palavra **seguinte** na frase introdutória. Por exemplo, considere as seguintes frases introdutórias:

> A lista a seguir identifica os principais parâmetros de desempenho:
>
> Siga os seguintes passos para instalar o pacote Frambus:
>
> A tabela a seguir resume os recursos de nosso produto em relação aos recursos de nossos principais concorrentes:

### Exercício

Escreva uma frase introdutória para a tabela a seguir:

<table class="table">
    <thead class="table-light">
        <tr>
            <th>Linguagens</th>
            <th>Inventor</th>
            <th>Ano Introduzido</th>
            <th>Recurso Principal</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Lisp</td>
            <td>John McCarthy</td>
            <td>1958</td>
            <td>recursão</td>
        </tr>
        <tr>
            <td>C++</td>
            <td>Bjarne Stroustrup</td>
            <td>1979</td>
            <td>OOP</td>
        </tr>
        <tr>
            <td>Python</td>
            <td>Guido van Rossum</td>
            <td>1994</td>
            <td>simplicidade</td>
        </tr>
    </tbody>
</table>

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Aqui estão algumas frases introdutórias possíveis para a tabela:</p>

<blockquote>A tabela a seguir contém alguns fatos importantes sobre algumas linguagens de programação populares:</blockquote>

<blockquote>A tabela a seguir identifica o inventor, ano de invenção e recurso principal de três linguagens de programação populares:</blockquote>

</details>

---

<p class="proxima-unidade"><b>Próxima unidade:</b> <a href="/curso/modulo-1/paragrafos/"><button type="button" class="btn btn-dark">Parágrafos</button></a></p>

{% include footer-conteudo-traduzido.html %}
