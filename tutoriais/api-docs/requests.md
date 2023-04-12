---
layout: tutorial-api-docs
title: Tutorial | Documentação de APIs - Exercício - Requests (Requisições)
permalink: /tutoriais/api-docs/requests/
---

# Exercício - Requests (requisições)

Ao final deste tópico, você terá a documentação dos **detalhes de requests** da API, seguindo as boas práticas desse tipo de conteúdo.

## Requests

Um **request** é uma solicitação feita para a API. A solicitação é uma forma de indicar para a API que você quer fazer alguma ação, como buscar ou inserir informações em uma base de dados, por exemplo. Uma API pode aceitar diversos tipos de requisições, por isso é importante detalhar todos os tipos possíveis na documentação.

A documentação de cada requisição deve conter estas informações:

* **Nome**
* **Método**
* **Path e endpoint**
* **Descrição**
* **Exemplo**

O **nome** da requisição precisa indicar o que ela faz. É uma boa prática iniciar o nome no infinitivo, como um verbo que indica uma ação. Por exemplo: listar, buscar, cadastrar, incluir, enviar.

É importante mencionar e descrever *todos* os **métodos** do request. Alguns requests aceitam somente um método, enquanto alguns podem aceitar vários métodos diferentes.

Ao citar o **path**, incluir a URL base é opcional, pois a URL já foi mencionada no início da documentação (considerando que você está seguindo este tutorial). Mas pode ser interessante incluir a URL base novamente junto com o path para facilitar testes com o endereço completo da requisição. Se você optar por incluir a URL base com o path, pode estilizar o texto para que a URL tenha menos destaque do que o path e o endpoint.

Na **descrição**, explique para que o endpoint é usado. Se o request para esse endpoint retorna algum dado na resposta, use a descrição para dar uma ideia geral do que é retornado. (Os detalhes da resposta serão documentados num tópico mais adiante do tutorial.)

Por fim, temos a documentação de um **request de exemplo**. O exemplo ajuda a demonstrar como fazer uma chamada para a API na prática. Normalmente o exemplo é escrito na forma de um comando [**cURL**](https://pt.wikipedia.org/wiki/CURL), o qual o desenvolvedor pode usar em um client como o Postman para testar o request.

Este é um exemplo dos elementos da documentação inicial de um request:

* **Listar os cadastros de usuários**
* **(GET) /integracao/listarUsuarios**
* **Busca a lista de usuários cadastrados no sistema e retorna os dados básicos dos perfis.**

No exemplo acima, `Listar os cadastros de usuários` é o **nome** do endpoint, `GET` é o **método** de requisição e `/integracao/listarUsuarios` é o **path** com o **endpoint**.

Apesar de o nome do endpoint ser bem explicativo (como deve ser), a **descrição** deixa ainda mais explícito o que esperar e dá uma ideia geral do que o request irá retornar.

## Exemplo prático

No [tópico anterior](/tutoriais/api-docs/nome-descricao-url/), começamos a documentação de uma API fictícia chamada **Gerenciador de Usuários**.

Suponha que a API Gerenciador de Usuários tem dois endpoints: um para buscar os **dados pessoais** e outro para os **dados de contato** dos usuários. Neste momento vamos documentar somente o endpoint de dados pessoais. Ao final do tutorial, adicionaremos o endpoint de dados de contato também.

Ambos os endpoints têm somente um método: o **GET**. Mas cada endpoint está em um **path** diferente.

* Documentação em Markdown:

> ```## Requests```
>
> ```### Requisição de exemplo```
>
> ``` `curl --location --request GET` ```
>
> ``` `'https://api.com.br/gerenciadorUsuarios/personal/getPersonalData' \` ```
> 
> ``` `--header 'Authorization: 1a2B3c4D5e' \` ```
> 
> ``` `--data-raw '{` ```
> 
> ``` `    "userId": 12345` ```
> 
> ``` `}'` ```
> 
> ```### Listar dados pessoais de usuários```
>
> ```(GET) /personal/getPersonalData```
>
> ```Retorna os **dados básicos do perfil** do usuário, com base em um identificador numérico único. O retorno inclui informações como o nome, data de nascimento e cor preferida, entre outras.```
> 
> ```### Listar dados de contato de usuários```
>
> ```(GET) /contact/getContatInformation```
>
> ```Retorna os **dados de contato do perfil** do usuário, com base em um identificador numérico único. O retorno inclui os números de telefone e endereços de e-mail do usuário```

Perceba que o endpoint **getPersonalData** está no path **/personal/**. Já o endpoint **getContactInformation** está no path **/contact/**. Usamos paths diferentes neste tutorial apenas para fins de exemplo, pois é comum que exista mais de um endpoint em um mesmo path. Esta é uma decisão arquitetural definida pelo time de engenharia do software quando a API está sendo projetada.

Ainda sobre o exemplo acima, inserimos o comando cURL de um exemplo funcional de requisição para a API. O desenvolvedor pode usar esse exemplo para fazer um request de teste e entender melhor como a API funciona.

Mais acima neste tutorial, falamos sobre a URL base ser opcional neste ponto da documentação. Aqui nós optamos por suprimir esta informação, mas ela poderia aparecer. Neste caso, a descrição dos paths seria assim:

> ```(GET) https://api.com.br/gerenciadorUsuarios/v1/personal/getPersonalData```
>
> ```(GET) https://api.com.br/gerenciadorUsuarios/v1/contact/getContatInformation```

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
> ### Requisição de exemplo
>
> `curl --location --request GET`
> `'https://api.com.br/gerenciadorUsuarios/personal/getPersonalData' \`
> `--header 'Authorization: 1a2B3c4D5e' \`
> `--data-raw '{`
> `"userId": 12345`
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

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/api-docs/header-body/"><button type="button" class="btn btn-dark">Exercício prático - Header e Body (cabeçalho e corpo)</button></a></p>
