---
layout: tutorial-api-docs
title: Tutorial | Documentação de APIs - Partes que compõem a documentação de APIs
permalink: /tutoriais/api-docs/partes-da-doc/
---

# Partes que compõem a documentação de APIs

Nesta seção do tutorial você vai conhecer:

* as principais partes que compõem a documentação de uma API
* quais informações cada parte precisa ter
* para que serve e como é usada cada parte da documentação da API

## Composição da documentação de APIs

Uma boa documentação de APIs é dividida em:

* Documentação conceitual
* Documentação de referência

## Documentação conceitual

A **documentação conceitual** deve ser uma introdução completa sobre a aplicação. Esta seção precisa conter pelo menos as seguintes informações:

* para que serve a API
* a quem se destina a API (ou stakeholders)
* o que a API pode fazer
* links para a documentação de referência

Adicionalmente, a documentação conceitual pode conter as seguintes informações:

* Casos de uso da API
* Códigos de exemplo, escritos nas linguagens de programação mais comuns ou naquelas que fizerem mais sentido para a aplicação
* O que a API *não* pode fazer (ou limitações que a API tem)
* Problemas conhecidos ou previstos que podem ocorrer durante a implementação da API
* Links para materiais complementares, tais como links externos, sites institucionais e tutoriais

Muitas vezes a documentação conceitual é negligenciada, mas ela tem o potencial de ser o fator decisivo na adoção da aplicação. Se uma pessoa não entende o que a API faz ou não tem certeza se ela atende ao que ela precisa, essa pessoa pode nem tentar usar a aplicação.

## Documentação de referência

A **documentação de referência** contém os seguintes detalhes dos requests:

* lista de requests que a API pode fazer
* como fazer cada request
* quais dados são retornados pelos requests

É comum encontrar documentações de APIs que focam somente na parte de referência, mas a parte conceitual é tão importante quanto. Quanto mais complexa é a API, mais importante é a seção conceitual.

As pessoas que vão desenvolver a aplicação estão divididas em dois perfis: há pessoas que gostam de partir direto para a prática e há também as pessoas que querem entender a fundo tudo sobre a API antes de começar a desenvolvê-la.

Normalmente, as pessoas que gostam mais da prática acessam a documentação de referência antes de tudo. No entanto, essas pessoas podem perceber que a API é mais complexa do que esperavam, ou podem ter dúvidas sobre regras e conceitos que não ficam explícitos na documentação de referência. Nesse momento, é útil ter a documentação conceitual disponível para resolver essas dúvidas. Outra ideia que costuma funcionar para este público é criar uma seção de **quick start** (início rápido), com um resumo dos conceitos e passos essenciais para criar uma primeira versão básica — mas funcional — da aplicação.

### Composição da documentação de referência

Normalmente, a documentação de referência é composta pelas seguintes partes:

* Nome e descrição da API
* URL base para fazer as requisições (requests)
* Lista de paths, incluindo métodos e endpoints
* Cabeçalho (Header) da requsição
* Corpo (Body) da requisição
* Responses (respostas)

Nos próximos tópicos, este tutorial irá guiar você pela documentação de cada uma dessas partes, até chegarmos na documentação completa de uma API fictícia.

Este tutorial assume que você conhece Markdown e a sintaxe de escrita desta linguagem.

O objetivo do tutorial é mostrar como uma documentação de API pode ser organizada num arquivo escrito em Markdown. Não é o objetivo deste tópico ensinar a sintaxe do Markdown e nem como escrever usando essa notação.

## Ferramentas necessárias

Este tutorial usará o [Markdown Online Editor (Dillinger.io)](https://dillinger.io/) - uma ferramenta online de edição e interpretação de Markdown. Mas você pode usar qualquer editor de texto e Markdown de sua preferência.

## Documentando cada parte da API

A seguir, este tutorial irá mostrar cada passo da construção de uma documentação de API usando Markdown. Cada seção tem um propósito bem definito e delimitado, o qual você aprender mais no tópico [Partes que compõem a documentação de APIs](/tutoriais/api-docs/partes-da-doc/).

A API de exemplo deste tutorial é bem simples, servindo para obter informações sobre usuários que estão cadastrados em um sistema fictício.