---
layout: tutorial-api-docs
title: Tutorial | Documentação de APIs - Exercício - Nome, descrição e URL
permalink: /tutoriais/api-docs/nome-descricao-url/
---

# Exercício - Nome, descrição e URL

Ao final deste tópico, você terá a documentação do **nome**, **descrição** e **URL** da API, seguindo as boas práticas desse tipo de conteúdo.

## Nome, descrição e URL

O **nome** da API deve aparecer em destaque no topo da documentação. O nome é a porta de entrada para a API, portanto ele precisa ser breve, mas explicativo.

A **descrição** da API deve ser um texto que resume o que ela faz e para que é usada. Se a API for muito complexa para concentrar todas as informações na descrição de introdução, faça links para a documentação conceitual, onde podem ser inseridas informações adicionais, desenhos de fluxos e diagramas.

A **URL base** é o endereço onde os serviços são executados. Na documentação da URL, forneça o endereço base da URL que será usada por cada endpoint para enviar os requests para a API. Se a API oferece mais de uma URL, descreva todas elas. Um exemplo comum em que há múltiplas URLs de uma mesma API é quando há uma para o ambiente de produção e outra para o ambiente de testes/homologação.

## Exemplo prático

Suponha que você precisa documentar uma API chamada **Gerenciador de Usuários**. Como o nome sugere, esta API é bem simples: ela permite administrar os usuários existentes num sistema de dados (digamos que sejam os usuários cadastrados num website).

Nesta primeira parte do tutorial, vamos construir uma documentação hipotética para a API fictícia **Gerenciador de Usuários**..

### Nome e descrição da API

A primeira parte da documentação contém o **nome** da API e uma **descrição** que resume o que ela faz.

* Documentação em Markdown:

> ```# Gerenciador de usuários```
>
> ```A API **Gerenciador de Usuários** é uma aplicação que permite integrar as informações de usuários cadastrados na base de dados.```
>
> ```As informações dos usuários estão categorizadas em **dois blocos**:```
> 
> ```* bloco de dados pessoais (`/getPersonalData`)```
> 
> ```* bloco de dados de contato (`/getContactInformation`)```
>
> ```Para obter os dados de cada bloco, você só precisa fazer uma requisição para o endpoint específico do bloco que quer consultar.```

### URL base

Esta seção deve descrever a URL que será usada para enviar os requests para a API. Todos os requests devem acontecer nessa URL, variando apenas o path e os endpoints contidos nela.

* Documentação em Markdown:

> ```## URL base```
>
> ``` `api.com.br/gerenciadorUsuarios/v1/` ```

## Resultado da documentação até aqui

Ao interpretar o conteúdo escrito em Markdown, teremos a seguinte saída:

> # Gerenciador de usuários
>
> A API **Gerenciador de Usuários** é uma aplicação que permite integrar as informações de usuários cadastrados na base de dados.
>
> As informações dos usuários estão categorizadas em **dois blocos**:
>
> * bloco de dados pessoais (`/getPersonalData`)
> * bloco de dados de contato (`/getContactInformation`)
>
> Para obter os dados de cada bloco, você só precisa fazer uma requisição para o endpoint específico do bloco que quer consultar.
>
> ## URL base
>
> `api.com.br/gerenciadorUsuarios/v1/`

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/api-docs/requests/"><button type="button" class="btn btn-dark">Exercício prático - Requests (requisições)</button></a></p>
