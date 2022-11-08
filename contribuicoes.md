# Contribuindo com o TW Livre

Para contribuir com o TW Livre (TWL), siga as orientações deste documento.

Se você nunca contribuiu ou não se sente confortável com o GitHub e open source, você pode praticar com o projeto [First Contributions](https://github.com/firstcontributions/first-contributions).

Antes de contribuir, leia também o [Código de Conduta do TWL](conduta.md).

## Issues

Antes de enviar um *pull request* (PR), veja se já existe uma issue relacionada ao que você vai fazer. Se a issue não existir, crie-a antes de enviar o PR.

### Sugerir algo ou relatar uma situação

Se você quer sugerir algo ou relatar um problema para o projeto, crie uma issue descrevendo a situação.

### Assumir ou criar uma issue

Se você se interessou por uma issue existente e acredita que pode tratá-la, atente-se a estes requisitos:

* prefira issues que tenham o label `help-wanted`
* se outra pessoa já estiver trabalhando na issue do seu interesse, pergunte se você pode ajudar

Se a situação que você vai tratar ainda não tem uma issue, crie uma e descreva a situação. Inclua pelo menos o *o que* você quer alterar e *qual* é o problema a ser corrigido ou melhoria a ser feita.

## Pull requests (PR)

### Vincular o PR a issues

* Se **já existem issues** para o assunto do seu PR, **vincule** as issues ao seu PR.
* Se **não existem issues** para o assunto do seu PR, **crie** as issues antes de enviar o PR. Ao enviar o PR, **vincule-o** às issues.

## Tipos de alteração

As contribuições no TWL podem ser alterações **funcionais** ou **de conteúdo**.

### Alterações funcionais

Uma alteração funcional envolve a arquitetura, interface e programação do [site do TWL](https://www.twlivre.org/).

Para saber quais frameworks e ferramentas o site usa, consulte a [documentação de tecnologias usadas pelo site](tecnologias.md).

> Contribuições com a arquitetura do site são muito bem-vindas. Ainda há muito para ser feito aqui — construí a base da melhor forma que eu pude, mas não sou web developer e nem web designer! :)

### Alterações de conteúdo

Uma alteração de conteúdo envolve mexer em:

* textos e guias do **curso essencial de Technical Writing**
* textos e guias dos **tutoriais**

Para saber quais frameworks e ferramentas foram usados para construir o conteúdo, consulte a [documentação de tecnologias usadas pelo site](tecnologias.md).

#### Curso essencial de Technical Writing

É o conteúdo existente na seção **Curso** do site.

O curso do TWL é uma tradução e adaptação do [treinamento de TW em inglês do Google](https://developers.google.com/tech-writing/)). Este curso tem dois módulos atualmente e o conteúdo programático de ambos está quase 100% fiéis ao original.

* O conteúdo do TWL está sob a licença de [Atribuição-NãoComercial-CompartilhaIgual 4.0 Internacional (**CC BY-NC-SA 4.0**)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.pt_BR). Qualquer contribuição feita ao projeto estará sujeita às condições desta licença.
* O conteúdo do curso original do Google está sob a licença de [Atribuição 4.0 Internacional (**CC BY 4.0**)](https://creativecommons.org/licenses/by/4.0/deed.pt_BR).

**Diretrizes gerais:**

> Idealmente, o conteúdo programático dos **dois primeiros módulos** do **curso** do TWL deve permanecer o mais fiel possível ao original em inglês. Nestes módulos, foque em **traduzir** e **corrigir** o que for necessário. Melhorias na **localização** e nos **exemplos** para o português brasileiro também são bem-vindos.
>
> Temas que não foram abordados nos dois primeiros módulos devem ser planejados para **novos módulos**. Novos módulos serão destinados a conteúdo criado exclusivamente para o TWL e que não existe no original do Google.
>
> O conteúdo deve ser escrito em Markdown. Exceções podem ser feitas para HTML, CSS e JavaScript nas situações em que não é possível usar Markdown, por exemplo quando é preciso aplicar estilos mais avançados.

#### Tutoriais / outros assuntos

Além do curso de essenciais em Technical Writing, o objetivo do projeto é reunir materiais adicionais que tenham alguma relação com TW.

Hoje o site conta somente com o curso essencial de Technical Writing, mas alguns tutoriais adicionais já estão sendo planejados.

Sugestões de temas são bem-vindas, mas procure ficar dentro dos seguintes assuntos:

* Ferramentas:
  * Jekyll e ferramentas similares
  * Content Management Systems (CMS)
  * Help Authoring Tools (HAT)
  * VSCode e outros editores de código
  * Git e GitHub
* Linguagens:
  * Markdown
  * HTML, CSS e JavaScript (com foco na criação de conteúdo)
* Processos:
  * Controle de versão e docs-as-code
  * Open source
* Técnicas:
  * Documentação de APIs
  * Guias de estilo de escrita (*Writing style guides*)
* Disciplinas:
  * UX Writing
  * Gestão do conhecimento
  * Arquitetura da informação

**Diretrizes gerais:**

> O conteúdo deve ser escrito em Markdown. Exceções podem ser feitas para HTML, CSS e JavaScript nas situações em que não é possível usar Markdown, por exemplo quando é preciso aplicar estilos mais avançados.
>
> Você pode melhorar tutoriais existentes, criar novas seções para eles ou criar tutoriais totalmente novos. Esta decisão pode ser feita em conjunto, visando a melhor arquitetura da informação do site.

## Guia de estilos e convenções

O guia de *writing*, formatação e estilos do site está em fase de construção. Para facilitar nessa parte, a revisão dos *pull requests* envolverá também o trabalho de edição e curadoria do conteúdo.

Até termos um guia de estilos, siga estas dicas:

* Procure seguir ao máximo os mesmos padrões de estilo dos documentos existentes.
* Siga as práticas essenciais do curso que está publicado no próprio site. Muitas das convenções usadas no site foram definidas com base no material do curso.
