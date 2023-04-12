---
layout: tutorial-api-docs
title: Tutorial | Documentação de APIs - Ferramentas para documentar APIs
permalink: /tutoriais/api-docs/ferramentas/
---

# Ferramentas para documentar APIs

Este tópico lista algumas ferramentas conhecidas que são usadas para documentar APIs. Tenha em mente que esta lista não é definitiva e nem delimitadora.

## Documentar APIs usando frameworks

Os frameworks de documentação de APIs facilitam a geração do conteúdo, pois trabalham com arquivos que seguem o padrão do Open API Specification (OAS).

Quando as pessoas estão desenvolvendo uma API, é possível gerar o arquivo na especificação OAS a partir do código-fonte contendo toda a documentação de referência dessa API. Então, os frameworks permitem importar o arquivo de especificação e gerar uma saída com a documentação formatada e organizada.

Existem frameworks gratuitos e pagos. Muitos deles permitem personalizar a aparência da documentação gerada, com diferentes níveis de personalização.

Estes são alguns frameworks conhecidos para gerar documentação de APIs:

* Gatsby — [site](https://www.gatsbyjs.com/)
* Jekyll — [site](https://jekyllrb.com/)
* Postman — [site](https://www.postman.com/)
* Redocly — [site](https://redocly.com/)
* Stoplight — [site](https://stoplight.io/)
* SwaggerHub — [site](https://swagger.io/)

## Documentar APIs em Markdown

O Markdown é uma linguagem bastante utilizada para criar documentação de APIs e software em geral, pelo fato de ser flexível e amplamente compatível com a metodologia *docs-as-code*.

Algumas das vantagens são:

* a popularidade da linguagem na área de desenvolvimento de software
* fácil de integrar documentação escrita em Markdown com conteúdo em outros formatos, como páginas em HTML
* flexibilidade para editar o conteúdo sem as "amarrações e regras" de um framework

Documentar APIs em Markdown facilita a criação de conteúdo conceitual sobre a API. Por outro lado, se a documentação de referência for escrita manualmente em Markdown, isso pode impedir ou dificultar a atualização, a automação e o compartilhamento do conteúdo. Por isso, o Markdown pode ser uma boa alternativa para escrever a documentação conceitual da API, mas pode não ser muito ágil para criar a documentação de referência. Outra dificuldade que pode aparecer é no caso de APIs extensas: quanto maior a API for e mais parâmetros ela tiver, mais trabalhoso vai ser criar a documentação de referência manualmente.

Por isso, uma boa prática é integrar o Markdown com o conteúdo do arquivo de especificação OAS. A documentação precisa evoluir junto com o produto e precisa de manutenção constante. Frameworks e ferramentas próprias para documentação têm recursos que facilitam a manutenção e a publicação do conteúdo.

### Ferramentas de edição em Markdown

O Markdown pode ser escrito em qualquer editor de texto convencional, mas existem ferramentas que permitem ver o resultado final do conteúdo enquanto estiver escrevendo. Estas são algumas dessas ferramentas:

* [Markdown Online Editor (Dillinger.io)](https://dillinger.io/)
* [Techscriptor](https://www.techscriptor.com/)
* [Visual Studio Code](https://code.visualstudio.com/) (quando usado em conjunto com extensões)

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/api-docs/partes-da-doc/"><button type="button" class="btn btn-dark">Partes que compõem a documentação de APIs</button></a></p>
