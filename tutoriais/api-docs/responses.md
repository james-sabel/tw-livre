---
layout: tutorial-api-docs
title: Tutorial | Documentação de APIs - Tutorial prático - Respostas
permalink: /tutoriais/api-docs/responses/
---

# Tutorial prático - Respostas

As respostas da requisição, também chamadas de **Responses**, são os dados que a API retorna depois de fazer a requisição. Portanto, essa seção deve descrever todos os dados que a API retorna ao fazer um request, incluindo os casos em que a requisição foi feita com **sucesso** e os que a requisição resultou em **erro**.

A resposta de uma requisição normalmente se enquadra em um dos seguintes cenários:

* um **código numérico** e uma **descrição** desse código, indicando se a requisição foi feita com sucesso ou com erros
* um **grupo de dados**, contendo as informações solicitadas pela requisição

No caso de retornar um **grupo de dados**, é importante incluir um exemplo da estrutura desses dados. O exemplo ajuda o desenvolvedor a manipular os dados retornados, pois fica mais claro como as informações estarão dispostas na resposta da API. Normalmente, o exemplo da resposta é apresentado na documentação no formato **JSON** (**JavaScript Object Notation**), por ser um dos mais usados pelos desenvolvedores e por serem fáceis de interpretar, mas existem outras maneiras de documentar.

## Exemplo prático

No [primeiro tópico do tutorial prático](/tutoriais/api-docs/nome-descricao-url/), começamos a documentação de uma API fictícia chamada **Gerenciador de Usuários**, a qual permite gerenciar os usuários cadastrados em um website. Também determinamos que essa API tem dois endpoints:

* `getPersonalData` - busca os **dados pessoais** dos usuários cadastrados no website.
* `getContatInformation`- busca os **dados de contato** dos usuários cadastrados no website.

Vamos documentar a resposta de cada um desses endpoints. Vamos supor que eles retornam os seguintes dados sobre o usuário cadastrado no website:

* `getPersonalData` (dados pessoais):
  * nome
  * data de nascimento
  * cidade e estado de residência
  * cor preferida
* `getContatInformation` (dados de contato):
  * número de telefone
  * endereço de e-mail
  * perfil de rede social

* Documentação em Markdown:

Vamos começar por alguns dos possíveis **códigos** de respostas da API. Vamos documentar apenas três códigos, mas lembre-se que existe uma lista extensa de códigos que uma requisição pode retornar. Você não precisa documentar todos os códigos, mas quanto mais você detalhar cada um na documentação, maior será a cobertura das situações que desenvolvedores possivelmente enfrentarão ao fazer uma requisição para a API.

> #### Respostas
> 
> | Código             | Descrição                                                                                                                                 |
> |--------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
> | `200 OK`           | A requisição foi feita corretamente e a API retornou os dados do usuário solicitados.                                                     |
> | `401 UNAUTHORIZED` | A requisição não foi autorizada. Certifique-se de ter incluído a chave de autenticação da API no Header da requisição.                    |
> | `404 NOT FOUND`    | Não foi possível encontrar o caminho especificado para a requisição. Verifique se a URL está correta e se o endpoint especificado existe. |

A única situação em que os endpoints conseguem retornar um grupo de dados será no retorno do código de sucesso - `200 OK`.

Cada endpoint retorna um grupo de dados diferente. (Não faria muito sentido dois endpoints distintos retornarem os mesmos dados, não é?) Por isso, vamos adicionar um exemplo no formato JSON para detalhar a resposta `200 OK` de cada endpoint separadamente.

* Documentação em Markdown:

> ```### Listar dados pessoais de usuários```
>
> ``` `(GET) /personal/getPersonalData` ```
>
> ```Retorna os **dados básicos do perfil** do usuário, com base em um identificador numérico único. O retorno inclui informações como o nome, data de nascimento e cor preferida, entre outras.```
> 
> ```#### Exemplo de resposta (`200 OK`)```
> 
> ``` > {  ```
> 
> ``` >   "name": "Adriana Silva", ```
> 
> ``` >   "birth": "02/05/1995", ```
> 
> ``` >   "city": "São Paulo/SP", ```
> 
> ``` >   "color": "Verde" ```
> 
> ``` > } ```
> 
> ```### Listar dados de contato de usuários```
>
> ``` `(GET) /contact/getContatInformation` ```
>
> ```#### Exemplo de resposta (`200 OK`)```
> 
> ``` > {  ```
> 
> ``` >  "phone": "+99 (99) 999-999-999", ```
> 
> ``` >  "email": "email@email.aa", ```
> 
> ``` >  "social": "@usuario - Nome da rede social" ```
> 
> ``` > } ```

## Resultado da documentação até aqui

Ao interpretar o conteúdo escrito em Markdown neste tópico e nas etapas anteriores do tutorial, teremos a seguinte saída:

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
> 
> ## Requests
> 
> ### Header
> **Authorization** `<appKey>`
> 
> Para obter a chave de autenticação (`appKey`), entre em contato com nosso Suporte ou gere sua própria chave pelo seu painel de administrador.
>
> ### Body
>
> | Parâmetro | Tipo    | Obrigatório | Descrição                                 |
> |-----------|---------|-------------|-------------------------------------------|
> | userId    | integer | Sim         | Código do identificador único do usuário. |
> 
> ### Requisição de exemplo
>
> `curl --location --request GET`
> 
> `'https://api.com.br/gerenciadorUsuarios/personal/getPersonalData' \`
> 
> `--header 'Authorization: 1a2B3c4D5e' \`
> 
> `--data-raw '{`
> 
> `"userId": 12345`
> 
> `}'`
> 
> ### Listar dados pessoais de usuários
>
>`(GET) /personal/getPersonalData`
>
> Retorna os **dados básicos do perfil** do usuário, com base em um identificador numérico único. O retorno inclui informações como o nome, data de nascimento e cor preferida, entre outras.
> 
> #### Respostas
> 
> | Código             | Descrição                                                                                                                                 |
> |--------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
> | `200 OK`           | A requisição foi feita corretamente e a API retornou os dados do usuário solicitados.                                                     |
> | `401 UNAUTHORIZED` | A requisição não foi autorizada. Certifique-se de ter incluído a chave de autenticação da API no Header da requisição.                    |
> | `404 NOT FOUND`    | Não foi possível encontrar o caminho especificado para a requisição. Verifique se a URL está correta e se o endpoint especificado existe. |
>
> #### Exemplo de resposta (`200 OK`)
> 
> > ```json
> > {
> >   "name": "Adriana Silva",
> >   "birth": "02/05/1995",
> >   "city": "São Paulo/SP",
> >   "color": "Verde"
> > }
> > ```
> 
> ### Listar dados de contato de usuários
>
> `(GET) /contact/getContatInformation`
>
> Retorna os **dados de contato do perfil** do usuário, com base em um identificador numérico único. O retorno inclui os números de telefone e endereços de e-mail do usuário.
> 
> #### Respostas
> 
> | Código             | Descrição                                                                                                                                 |
> |--------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
> | `200 OK`           | A requisição foi feita corretamente e a API retornou os dados do usuário solicitados.                                                     |
> | `401 UNAUTHORIZED` | A requisição não foi autorizada. Certifique-se de ter incluído a chave de autenticação da API no Header da requisição.                    |
> | `404 NOT FOUND`    | Não foi possível encontrar o caminho especificado para a requisição. Verifique se a URL está correta e se o endpoint especificado existe. |
>
> #### Exemplo de resposta (`200 OK`)
>
> > ```json
> > {
> >   "phone": "+99 (99) 999-999-999",
> >   "email": "email@email.aa",
> >   "social": "@usuario - Nome da rede social"
> > }
> > ```