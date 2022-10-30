---
layout: curso-modulo-1
title: Pontuação (Opcional)
permalink: /curso/modulo-1/pontuacao/
---

# Pontuação (Opcional)

<div class="alerta alerta-simples">
    <p>Tempo estimado: 5 minutos</p>
</div>

Esta unidade opcional fornece uma atualização rápida dos sinais de pontuação.

## Vírgulas

As linguagens de programação impõem regras claras sobre pontuação. Em português, por outro lado, as regras sobre vírgulas são um pouco mais nebulosas. Como diretriz, insira uma vírgula sempre que um leitor pausaria naturalmente em algum lugar dentro de uma frase. A pausa para uma vírgula é mais curta do que para um ponto final. Por exemplo, se você ler a frase a seguir em voz alta, provavelmente descansará brevemente antes da palavra *apenas*:

> C se comporta como uma linguagem de nível médio, apenas alguns passos acima na abstração da linguagem assembly.

Algumas situações requerem uma vírgula. Por exemplo, use vírgulas para separar itens em uma lista incorporada como a seguir:

> Nossa empresa usa C++, Python, Java, e JavaScript.

Você pode estar se perguntando sobre a vírgula final de uma lista, aquela inserida entre os itens N-1 e N. Essa vírgula – conhecida como **vírgula serial** ou **vírgula de Oxford** – é controversa. Ela é mais comum na língua inglesa do que na portuguesa. No português, fornecer essa vírgula final pode ser uma boa ideia simplesmente porque a redação técnica exige a escolha da solução menos ambígua. Dito isso, preferimos contornar a controvérsia convertendo listas incorporadas em listas com marcadores.

Nas frases que expressam uma condição, coloque uma vírgula entre a condição e a consequência. Por exemplo, ambas as frases a seguir fornecem a vírgula no lugar correto:

> Se o programa estiver lento, use o parâmetro `--perf`.
>
> Se o programa estiver lento, então use o parâmetro `--perf`.

Você também pode colocar uma definição rápida ou digressão entre um par de vírgulas, como no exemplo a seguir:

> Python, uma linguagem fácil de usar, ganhou impulso significativo nos últimos anos.

Finalmente, evite usar uma vírgula para colar dois pensamentos independentes. Por exemplo, a vírgula na frase a seguir é culpada de um crime de pontuação chamado **emenda de vírgula**:

<i class="fa fa-thumbs-down" style="color: #DD2C00"></i> <b>Não recomendado</b>

> Samantha é uma programadora maravilhosa, ela escreve muitos cenários de testes.

Use um ponto em vez de uma vírgula para separar dois pensamentos independentes. Por exemplo:

<i class="fa fa-thumbs-up" style="color: #34A853"></i> <b>Recomendado</b>

> Samantha é uma programadora maravilhosa. Ela escreve muitos cenários de testes.

### Exercício

Adicione vírgulas quando apropriado à seguinte passagem:

> Os Buffers de Protocolo às vezes conhecidos como protobufs são o principal formato de dados estruturados de nossa equipe. Use Buffers de Protocolo para representar armazenar e transferir dados estruturados. Ao contrário do XML os Buffers de Protocolo são compilados. Consequentemente os clientes transmitem os Buffers de Protocolo de forma eficiente o que levou à rápida adoção.

Dica: Leia a passagem em voz alta e coloque uma vírgula em todos os lugares onde você ouvir uma pequena pausa.

<details>
<summary>Clique para revelar a resposta.</summary>

<p>Aqui está uma solução possível:</p>

<blockquote>Os Buffers de Protocolo, às vezes conhecidos como protobufs, são o principal formato de dados estruturados de nossa equipe. Use Buffers de Protocolo para representar, armazenar e transferir dados estruturados. Ao contrário do XML, os Buffers de Protocolo são compilados. Consequentemente, os clientes transmitem os Buffers de Protocolo de forma eficiente, o que levou à rápida adoção.</blockquote>

</details>

## Ponto e vírgula

Um ponto final separa pensamentos distintos; um ponto e vírgula une pensamentos altamente relacionados. Por exemplo, observe como o ponto e vírgula na frase a seguir une o primeiro e o segundo pensamento:

<i class="fa fa-thumbs-up" style="color: #34A853"></i> <b>Recomendado</b>

> Execute novamente o Frambus após atualizar seu arquivo de configuração; não execute novamente o Frambus após atualizar o código-fonte existente.

Antes de usar um ponto e vírgula, pergunte a si mesmo se a frase ainda faria sentido se você invertesse os pensamentos para lados opostos do ponto e vírgula. Por exemplo, inverter o exemplo anterior ainda produz uma sentença válida:

> Não execute novamente o Frambus após atualizar o código-fonte existente; execute novamente o Frambus após atualizar seu arquivo de configuração.

Os pensamentos que precedem e seguem o ponto e vírgula devem ser sentenças gramaticalmente completas. Por exemplo, o ponto e vírgula a seguir está incorreto porque a passagem após o ponto e vírgula é uma cláusula, não uma frase completa:

<i class="fa fa-thumbs-down" style="color: #DD2C00"></i> <b>Não recomendado</b>

> Execute novamente o Frambus após atualizar seu arquivo de configuração; não depois de atualizar o código-fonte existente.

<i class="fa fa-thumbs-up" style="color: #34A853"></i> <b>Recomendado</b>

> Execute novamente o Frambus após atualizar seu arquivo de configuração, não após atualizar o código-fonte existente.

Você quase sempre deve usar vírgulas, não ponto e vírgula, para separar itens em uma lista incorporada. Por exemplo, o seguinte uso de ponto e vírgula está incorreto:

<i class="fa fa-thumbs-down" style="color: #DD2C00"></i> <b>Não recomendado</b>

> Os guias de estilo são maiores que a lua; mais essencial que o oxigênio; e completamente incompreensíveis.

Conforme mencionado anteriormente nesta lição, a redação técnica geralmente prefere listas com marcadores do que listas incorporadas. No entanto, se você realmente preferir uma lista incorporada, use vírgulas em vez de ponto e vírgula para separar os itens, como no exemplo a seguir:

<i class="fa fa-thumbs-up" style="color: #34A853"></i> <b>Recomendado</b>

> Os guias de estilo são maiores que a lua, mais essenciais que o oxigênio e completamente incompreensíveis.

Muitas frases colocam uma palavra ou frase de conjunção imediatamente após o ponto e vírgula. Nesta situação, coloque uma vírgula após a conjunção. Observe a vírgula após a conjunção nos dois exemplos a seguir:

> O Frambus não fornece nenhum pacote oficial de código aberto para manipulação de strings; entretanto, subconjuntos de pacotes de manipulação de strings estão disponíveis em outros projetos de código aberto.
>
> Mesmo as mudanças de código aparentemente triviais podem causar bugs; portanto, escreva testes unitários abundantes.

### Exercício

Qual dos seguintes pontos finais ou vírgulas você poderia substituir por um ponto e vírgula?

1. Python é uma linguagem de programação popular. A linguagem C foi desenvolvida muito antes do Python.
2. O aprendizado do modelo para um valor baixo de X aparece na ilustração superior. O aprendizado do modelo para um valor alto de X aparece na ilustração inferior.
3. Sou grato pelo meu monitor grande, CPU poderosa e largura de banda incrível.

<details>
<summary>Clique para revelar a resposta.</summary>

<ol>
   <li>Você não pode converter o ponto final do #1 para um ponto e vírgula porque as duas frases são apenas vagamente relacionadas.</li>
   <li>Você pode substituir o ponto final do #2 por um ponto e vírgula porque as duas frases são altamente relacionadas.</li>
   <li>Você não pode converter as vírgulas do #3 para ponto e vírgula. Use vírgulas para separar itens em uma lista incorporada.</li>
</ol>

</details>

## Travessões

Os travessões são sinais de pontuação atraentes, ricos em possibilidades de pontuação. Um travessão representa uma pausa mais longa – uma pausa maior – do que uma vírgula. Por exemplo:

> C++ é uma linguagem rica – que requer uma vasta experiência para dominar.

Às vezes, os redatores usam um par de travessões para isolar uma digressão, como no exemplo a seguir:

> Buffers de Protocolo — muitas vezes apelidados de protobufs — codificam dados estruturados em um formato eficiente e extensível.

Poderíamos ter usado vírgulas em vez de travessões nos exemplos anteriores? Claro. Por que escolhemos um travessão em vez de uma vírgula? Instinto. Arte. Experiência.

### Travessões e hífens

Considere os sinais de pontuação horizontais mostrados na tabela a seguir:

<table class="table">
    <thead class="table-light">
        <tr>
            <th>Nome</th>
            <th>Marcação</th>
            <th>Largura relativa</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>travessão</td>
            <td>—</td>
            <td>mais largo (geralmente, o comprimento da letra m)</td>
        </tr>
        <tr>
            <td>meia-risca (traço)</td>
            <td>–</td>
            <td>médio (geralmente, o comprimento da letra n)</td>
        </tr>
        <tr>
            <td>hífen</td>
            <td>-</td>
            <td>mais estreito</td>
        </tr>
    </tbody>
</table>

Alguns guias de estilo recomendam o travessão para determinados usos. O Guia de Estilo do Google, no entanto, oferece os seguintes conselhos sobre travessões: não use.

**Hífens** são complicados. Dentro da escrita técnica, os hífens conectam palavras em certos termos compostos, como:

> público-alvo

Em caso de dúvida sobre hífens, consulte um dicionário, glossário ou guia de estilo.

<div class="alerta alerta-azul">
    <p>Se você consultar mais de um dicionário, glossário ou guia de estilo sobre hífens, poderá encontrar inconsistências.</p>
</div>

## Parênteses

Use parênteses para passar ideias curtas e digressões. Os parênteses informam aos leitores que o texto incluído não é crítico. Como o texto incluído não é crítico, alguns editores acham que o texto que merece parênteses não merece estar no documento. Comprometa-se a reduzir os parênteses a um mínimo na redação técnica.

As regras sobre pontos finais e parênteses nem sempre são claras. Aqui estão as regras padrão:

> Se um par de parênteses contém uma frase inteira, o ponto vai para dentro do parêntese de fechamento.
>
> Se um par de parênteses termina uma frase, mas não contém a frase inteira, o ponto vai para fora do parêntese de fechamento.

Por exemplo:

> (Aliás, os buffers de protocolo são ótimos presentes de aniversário.)
>
> O modo binário depende da forma nativa mais compacta (descrita posteriormente neste documento).

---

<p class="proxima-unidade"><b>Próxima unidade:</b> <a href="/curso/modulo-1/markdown/"><button type="button" class="btn btn-dark">Markdown</button></a> (opcional)</p>

{% include footer-conteudo-traduzido.html %}
