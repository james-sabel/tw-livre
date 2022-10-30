---
layout: curso-modulo-2
title: Criando código de exemplo
permalink: /curso/modulo-2/codigo-exemplo/
---

# Criando código de exemplo

<div class="alerta alerta-simples">
    <p>Tempo estimado: 10 minutos</p>
</div>

Um bom código de exemplo geralmente é a melhor documentação. Mesmo que seus parágrafos e listas sejam claros, os programadores ainda preferem um bom código de amostra. Afinal, texto e código são linguagens diferentes, e é com código que o leitor se preocupa. Tentar descrever código com texto é como tentar explicar um poema italiano em inglês.

Boas amostras são códigos **corretos** e **concisos** que seus leitores podem **entender rapidamente** e **reutilizar facilmente** com **efeitos colaterais mínimos**.

## Correto

O código de exemplo deve atender aos seguintes critérios:

* Compilar sem erros.
* Executar a tarefa que ele afirma realizar.
* Estar o mais pronto possível para a produção. Por exemplo, o código não deve conter nenhuma vulnerabilidade de segurança.
* Seguir as convenções específicas da linguagem.

O código de exemplo é uma oportunidade de influenciar diretamente como seus usuários escrevem código. Portanto, o código de exemplo deve definir a melhor maneira de usar seu produto. Se houver mais de uma maneira de codificar a tarefa, codifique-a da maneira que sua equipe decidiu ser a melhor. Se sua equipe não considerou os prós e os contras de cada abordagem, reserve um tempo para fazê-lo.

Sempre teste seu código de exemplo. Com o tempo, os sistemas mudam e seu código de exemplo pode falhar. Esteja preparado para testar e manter o código de exemplo como faria com qualquer outro código.

Muitas equipes reutilizam seus testes unitários como programas de exemplo, o que às vezes é uma má ideia. O objetivo principal de um teste unitário é testar; o único objetivo de um programa de exemplo é educar.

Um *snippet* é um trecho de código de um programa de exemplo, possivelmente com apenas uma ou algumas linhas. A documentação com muitos *snippets* geralmente se degrada com o tempo porque as equipes tendem a não testar os *snippets* com tanto rigor quanto os programas de exemplo completos.

### Executando código de exemplo

Bons documentos explicam como executar código de exemplo. Por exemplo, seu documento pode precisar instruir os usuários a realizar atividades como as seguintes, antes de executar os exemplos:

* Instalar uma determinada biblioteca.
* Ajustar os valores atribuídos a determinadas variáveis ​​de ambiente.
* Ajustar algo no ambiente de desenvolvimento integrado (IDE).

Os usuários nem sempre executam as atividades anteriores corretamente. Em algumas situações, os usuários preferem executar ou (experimentar) código de exemplo diretamente na documentação. ("Clique aqui para executar este código.")

Os redatores devem considerar descrever a saída ou resultado esperado do código de exemplo, especialmente para código de exemplo difícil de executar.

## Conciso

O código de exemplo deve ser curto, incluindo apenas componentes essenciais. Quando um programador C iniciante quiser aprender como chamar a função `malloc`, dê a esse programador um breve trecho, não toda árvore do código-fonte do Linux. Código irrelevante pode distrair e confundir seu público. Dito isso, nunca use más práticas para encurtar seu código; sempre prefira o correto ao conciso.

## Compreensível

Siga estas recomendações para criar um código de exemplo claro:

* Escolha nomes descritivos de classes, métodos e variáveis.
* Evite confundir seus leitores com truques de programação difíceis de decifrar.
* Evite código profundamente aninhado.
* Opcional: Use fonte em negrito ou colorida para chamar a atenção do leitor para uma seção específica do seu código de exemplo. No entanto, use o destaque criteriosamente – muito destaque significa que o leitor não se concentrará em nada em particular.

### Exercício

Qual das opções a seguir seria uma linha de código mais útil em um programa de exemplo? Suponha que o público-alvo seja formado por engenheiros de software novos na API fictícia `go.so`.

1. `MeuNivel = go.so.Nivel(5, 28, 48)`
2. `MeuNivel = go.so.Nivel(ranque=5, 28, 48)`
3. `MeuNivel = go.so.Nivel(ranque=5, dimensao=28, opacidade=48)`

<details>
<summary>Clique para revelar a resposta.</summary>

<p>A resposta <b>3</b> é a melhor escolha aqui. Embora seja tentador manter o código de exemplo o mais curto possível, a omissão de nomes de parâmetros dificulta o aprendizado dos novatos.</p>

</details>

## Comentado

Considere as seguintes recomendações sobre comentários no código de exemplo:

* Mantenha os comentários curtos, mas sempre prefira a clareza à brevidade.
* Evite escrever comentários sobre código óbvio, mas lembre-se de que o que é óbvio para você (o especialista) pode não ser óbvio para os novatos.
* Concentre sua energia de comentários em qualquer coisa não intuitiva no código.
* Quando seus leitores são muito experientes com uma tecnologia, não explique *o que* o código está fazendo, explique *por que* o código está fazendo isso.

Você deve colocar descrições de código dentro de comentários de código ou em texto (parágrafos ou listas) fora do código de exemplo? Observe que os leitores que copiam e colam um *snippet* coletam não apenas o código, mas também os comentários incorporados. Portanto, coloque quaisquer descrições que pertençam ao código colado nos comentários do código. Por outro lado, quando você precisa explicar um conceito longo ou complicado, normalmente deve colocar o texto antes do programa de amostra.

<div class="alerta alerta-azul">
    <p>Se você precisar deixar o código menos pronto para a produção para torná-lo mais curto e fácil de entender, explique suas decisões nos comentários.</p>
</div>

### Exercício

Quais problemas você vê nos comentários no *snippet* a seguir? Suponha que o código seja voltado para programadores que são novos na API `br`, mas que têm alguma experiência com o conceito de *streams*:

```java
/* Cria um fluxo a partir do arquivo de texto do caminho /tmp/myfile. */
mystream = br.openstream(pathname="/tmp/myfile", mode="z")
```

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Os comentários contêm as seguintes falhas:</p>

<ul>
    <li>O comentário elabora uma parte bastante óbvia do código.</li>
    <li>O <i>snippet</i> não explica a parte não óbvia do código. Ou seja, o que é o parâmetro <code>mode</code> e o que significa um valor de "z"?</li>
</ul>

</details>

## Reutilizável

Para que seu leitor reutilize facilmente seu código de exemplo, forneça o seguinte:

* Todas as informações necessárias para executar o código de exemplo, incluindo quaisquer dependências e configuração.
* Código que pode ser estendido ou personalizado de maneiras úteis.

Ter um código de exemplo fácil de entender, conciso e compilado é um ótimo começo. Porém, se o aplicativo dos seus leitores explodir, eles não ficarão felizes. Portanto, ao escrever o código de exemplo, considere quaisquer efeitos colaterais potenciais causados ​​pela integração do seu código em outro programa. Ninguém quer um código inseguro ou extremamente ineficiente.

## O exemplo e o anti-exemplo

Além de mostrar aos leitores *o que fazer*, às vezes é sábio mostrar aos leitores *o que não fazer*. Por exemplo, muitas linguagens de programação permitem que os programadores coloquem espaços em branco em ambos os lados do sinal de igual. Agora suponha que você esteja escrevendo um tutorial em uma linguagem (como *bash*) que não permite espaço em branco em ambos os lados do sinal de igual. Nesse caso, mostrar um bom exemplo e um anti-exemplo beneficiará o leitor. Por exemplo:

<i class="fa fa-thumbs-up" style="color: #34A853"></i>

```text
# Uma atribuição de string válida.
s="A chuva no Maine."
```

<i class="fa fa-thumbs-down" style="color: #DD2C00"></i>

```text
# Uma atribuição de string inválida devido ao espaço em branco em ambos os lados do
# sinal de igual.
s = "A chuva no Maine."
```

## Sequenciado

Um bom conjunto de códigos de exemplo demonstra uma variedade de complexidade.

Leitores completamente não familiarizados com uma determinada tecnologia normalmente desejam exemplos simples para começar. O primeiro e mais básico exemplo em um conjunto de códigos de amostra geralmente é chamado de [programa Olá Mundo](https://pt.wikipedia.org/wiki/Programa_Ol%C3%A1_Mundo). Depois de dominar o básico, os engenheiros de software querem programas mais complexos. Um bom conjunto de códigos de exemplo fornece uma gama saudável de programas de exemplo simples, moderados e complexos.

### Exercício

Qual das opções a seguir seria um bom conjunto de funções de exemplo para apoiar um tutorial apresentando o conceito de funções a novatos?

<ol>
    <li>O seguinte conjunto de funções:
        <ul style="list-style-type: lower-alpha;">
            <li>Uma função que não recebe parâmetros e não retorna nada.</li>
            <li>Uma função que recebe um parâmetro, mas não retorna nada.</li>
            <li>Uma função que recebe um parâmetro e retorna um valor.</li>
            <li>Uma função que recebe três parâmetros e retorna um valor.</li>
        </ul>
    </li>
    <li>O seguinte conjunto de funções:
        <ul style="list-style-type: lower-alpha;">
            <li>Uma função que recebe três parâmetros e retorna um valor.</li>
        </ul>
    </li>
    <li>O seguinte conjunto de funções:
        <ul style="list-style-type: lower-alpha;">
            <li>Uma função que recebe um parâmetro e retorna um valor.</li>
            <li>Uma função que recebe três parâmetros e retorna um valor.</li>
        </ul>
    </li>
</ol>

<details>
<summary>Clique para revelar a resposta.</summary>

<p>A melhor resposta é <b>1</b>. Fornecer amostras que cobrem uma faixa de complexidade geralmente é a escolha mais sábia, principalmente para os recém-chegados. Resista à tentação de <i>correr</i> para programas de amostra muito complexos, ignorando os programas de amostra para iniciantes e intermediários que os recém-chegados querem.</p>

</details>

## O que vem a seguir?

Parabéns: você concluiu o conteúdo do Módulo 2.

Uma rápida compilação dos tópicos abordados no Módulo 2 está disponível na página [Resumo](/curso/modulo-2/resumo/).

{% include footer-conteudo-traduzido.html %}
