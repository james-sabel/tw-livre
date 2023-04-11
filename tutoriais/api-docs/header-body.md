---
layout: tutorial-api-docs
title: Tutorial | Documentação de APIs - Tutorial prático - Cabeçalho e Corpo
permalink: /tutoriais/api-docs/header-body/
---

# Tutorial prático - Cabeçalho e Corpo

## Cabeçalho

O cabeçalho da requisição, também chamado de **Header**, é uma lista de todos os parâmetros que devem aparecer no início do request feito para a API. É a primeira informação que a API espera receber antes das informações principais, as quais estarão mais adiante no corpo da requisição.

Se uma pessoa precisa usar algum tipo de autenticação (API Key, OAuth, Bearer, etc.), mencione isso nesta parte da documentação.

Forneça qualquer informação adicional que alguém pode precisar para que o request funcione. Por exemplo: se a pessoa precisa obter alguma credencial ou uma API Key de autorização, explique onde e como são obtidas.

## Corpo

O corpo da requisição, também chamado de **Body**, é uma lista de todos os parâmetros que contém os principais dados de entrada do request. Isso significa que você pode (e em alguns casos você *deve*) enviar um dado inicial para que a API saiba o que devolver na resposta.

A documentação de cada parâmetro do Body precisa ter pelo menos estas informações:

* Nome do parâmetro
* Tipo de dado (string, integer, boolean, etc.) esperado pelo parâmetro
* Obrigatoriedade do parâmetro
* Descrição do parâmetro

Às vezes os parâmetros do Body são chamados de **parâmetros de entrada** ou de *Input*. Eles levam esse nome porque são informações que o usuário da API deve fornecer para que ela possa processar a requisição.

## Obrigatoriedade

Nem toda requisição exige que dados sejam enviados no Header ou no Body.

Existem APIs que não exigem nenhum tipo de autenticação e não esperam nenhuma informação de entrada para poder retornar uma resposta. Existem também APIs que tornam os parâmetros de entrada como opcionais, devolvendo respostas diferentes dependendo do que foi informado.

Exemplo (clique para expandir):

Imagine uma API que retorna os dados pessoais de usuários cadastrados em um site. Gostaríamos de acreditar que uma API como essa não deixaria os dados abertos para qualquer pessoa e exigiria algum tipo de **autenticação** no **Header**.

Faz sentido acreditar também que o site tenha um número grande de usuários cadastrados. Nesse caso, uma API como essa provavelmente exigirá que o **Body** da requisição contenha pelo menos um **parâmetro** que permita você restringir quais usuários quer consultar. Esse cenário costuma ter duas alternativas:

* A API pode tornar o parâmetro **obrigatório** e retornar um erro se ele não for enviado na requisição.
* A API pode manter o parâmetro **opcional**: se ele for informado, a API retornará as informações dos usuários que se enquadram no critério definido; se ele não for informado, a API retornará as informações de todos os usuários cadastrados.

## Exemplo prático

No [primeiro tópico do tutorial prático](/tutoriais/api-docs/nome-descricao-url/), começamos a documentação de uma API fictícia chamada **Gerenciador de Usuários**.

Suponha que a API Gerenciador de Usuários tem as seguintes características:

* Requisições para essa API exigem uma autenticação feita via API Key
* Ambos os endpoints - documentados no [tópico anterior deste tutorial](/tutoriais/api-docs/requests/) - esperam algum tipo de identificador único do usuário para retornar os dados dele

Como a API espera uma chave (API Key), é indispensável que a documentação deixe claro onde obter essa chave. Caso contrário, o desenvolvedor ficará impedido de seguir com a implementação.

* Documentação em Markdown:

> ```### Header```
> 
> ```**Authorization** `<appKey>````
> 
> ```Para obter a chave de autenticação (`appKey`), entre em contato com nosso Suporte ou gere sua própria chave pelo seu painel de administrador.```
>
> ```### Body```
>
> ```| Parâmetro | Tipo    | Obrigatório | Descrição                                 |```
> 
> ```|-----------|---------|-------------|-------------------------------------------|```
> 
> ```| userId    | integer | Sim         | Código do identificador único do usuário. |```

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
> ### Listar dados de contato de usuários
>
> `(GET) /contact/getContatInformation`
>
> Retorna os **dados de contato do perfil** do usuário, com base em um identificador numérico único. O retorno inclui os números de telefone e endereços de e-mail do usuário.

### Sobre a solução apresentada neste tutorial

Perceba que as informações do Header e do Body foram adicionadas antes da lista de Endpoints. Essa foi uma escolha deste tutorial, porque imaginamos que a nossa API fictícia Gerenciador de Usuários usa o mesmo tipo de autenticação e os mesmos parâmetros de entrada para todos os Endpoints. Se cada Endpoint tivesse autenticações e entradas distintas, talvez fosse uma boa ideia que cada Endpoint tivesse sua própria seção de Header e Body.

O que vai variar entre os Endpoints são os dados que retornam nas **respostas** (ou *Responses*) de cada um. Vamos tratar essa parte na próxima etapa deste tutorial.