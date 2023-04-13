---
layout: tutorial-api-docs
title: Tutorial | Documentação de APIs - Introdução a APIs
permalink: /tutoriais/api-docs/introducao-apis/
---

# Introdução a APIs

Este tópico apresenta um conceito geral para começar a entender o que são APIs, a lógica por trás delas e alguns termos comuns.

A compreensão dos conceitos básicos descritos aqui ajudarão você a seguir com o tutorial de documentação de APIs com mais clareza e fluidez.

## O que são APIs

**APIs** são ecossistemas de **ferramentas** e **recursos** que permitem que desenvolvedores criem software que se comunica com outros softwares. O nome API é a abreviação de **Application Programming Interface**, o que em tradução livre para o português significa **Interface de Programação de Aplicativos**.

Um exemplo comum de comunicação feita usando APIs acontece ao enviar os dados de pagamento num site de compras. Ao fazer isso, o site irá usar APIs para enviar e validar os dados do cartão de crédito com a instituição operadora do cartão. Da mesma forma, o site vai usar APIs para obter o retorno da operadora, com a aprovação ou rejeição da transação com o cartão.

<p style="text-align: center; margin-top: 40px; margin-bottom: 40px;">
    <img src="/res/img/api-docs/conceito-01.png" alt-text="Exemplo de comunicação entre loja virtual e operadora de cartão de crédito" title="Exemplo de comunicação entre loja virtual e operadora de cartão de crédito" />
</p>

Para tornar essa comunicação possível, desenvolvedores precisam de informações específicas sobre a API, como os dados esperados por ela e quais informações serão retornadas por ela em cada comunicação.

A comunicação usando APIs sempre ocorre **entre um cliente e um servidor**. O cliente é o lado que inicia a comunicação e faz a solicitação de uma informação, enquanto o servidor é o lado que recebe a solicitação e devolve uma resposta.

## APIs públicas e privadas

Uma API pode ser **pública** ou **privada**.

Como os nomes sugerem, APIs públicas são abertas e podem receber requisições externas de qualquer origem. Uma API pública pode ser totalmente aberta e receber requisições sem nenhum tipo de autorização especial, mas também pode exigir alguma autenticação. Tudo depende de como ela foi construída e do seu objetivo. Já as APIs privadas são de uso interno e não ficam disponíveis para o público em geral.

No cenário de uma empresa desenvolvedora de software, ela pode criar **APIs privadas** que serão usadas apenas dentro da organização. Assim, os sistemas dessa empresa podem enviar e receber dados entre si, internamente.

Por outro lado, a empresa pode disponibilizar **APIs públicas** para permitir que desenvolvedores externos criem aplicativos, produtos e soluções que se integram ao sistema da empresa. Com essa integração, desenvolvedores podem criar funcionalidades que agregam novos recursos ao software original, criando novas soluções para seus usuários.

## Tipos e arquiteturas de API

Os tipos de API são definidos pela sua **arquitetura**. A arquitetura de uma API é a maneira como ela é construída e como ela faz a comunicação entre os sistemas.

Estas são as arquiteturas de API mais populares atualmente, mas existem outras:

* **REST** (Representational State Transfer)
* **SOAP** (Simple Object Access Protocol)
* **GraphQL**
* **gRPC** (Google Remote Procedure Call)

Cada arquitetura tem suas próprias vantagens e desvantagens e são usadas em diferentes cenários, dependendo das necessidades de negócio e do projeto de atuação.

Aqui no tutorial do TW Livre vamos falar somente sobre a documentação de APIs que seguem a arquitetura **REST**, por causa da sua popularidade e aplicação nos dias atuais.

### API REST

Existem diversas maneiras de um cliente enviar uma solicitação para um servidor usando APIs. No caso das APIs REST, a solicitação é feita usando um **protocolo HTTP**. Cada solicitação é chamada de **requisição**, também conhecida como **request**. (Este tutorial usa os termos de forma intercambiável. "Requisição", "request" e "solicitação" signficam a mesma coisa aqui.)

<p style="text-align: center; margin-top: 20px; margin-bottom: 20px;">
    <img src="/res/img/api-docs/conceito-02.png" alt-text="Diagrama de comunicação de uma API REST" title="Diagrama de comunicação de uma API REST" />
</p>

O protocolo HTTP é uma maneira de representar a interação do cliente com o servidor. Esse protocolo é responsável por dizer *como* o request precisa ser feito, de forma que o servidor entenda:

* o que foi solicitado
* quais recursos a API está solicitando
* o tipo de operação da solicitação, como adicionar ou excluir um recurso, por exemplo

O tipo de operação da solicitação é chamado de **método**. Métodos são representados por verbos, pois executam alguma ação no recurso que se encontra no servidor.

Estes são os métodos mais comuns de um protocolo HTTP:

* **GET** - *buscar* uma informação do servidor, retornando dados como resposta da requisição.
* **POST** - *enviar* uma informação para o servidor. Normalmente causa alguma mudança de estado no recurso que se encontra no servidor.
* **DELETE** - *excluir* uma informação do servidor.

Além dos métodos acima, existem também outros: **HEAD**, **PUT**, **CONNECT**, **OPTIONS**, **TRACE** e **PATCH**.

Você pode consultar a [documentação de métodos de requisições HTTP no site MDN Web Docs](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Methods).

Depois de processar o request com um dos métodos acima, a API devolve uma resposta (também usando o protocolo HTTP) que contém as informações resultantes da solicitação. Cada retorno devolvido pela API é chamado de **resposta**, ou **response**. (Este tutorial usa os termos de forma intercambiável. "Resposta" e "response" signficam a mesma coisa aqui.)

### Autenticação em API REST

Algumas APIs do tipo REST, especialmente as APIs privadas, exigem algum tipo de **autenticação** antes de receber um request. A autenticação garante a segurança das comunicações entre a aplicação e a API.

Um dos meios de autenticação mais comuns é a **API Key**: um código alfanumérico que indica que a pessoa fazendo a requisição tem acesso aos recursos da API. Mas existem diversos outros meios de autenticação, os quais são analisados pelo time de engenharia e definidos no momento da implementação. Cada tipo de autenticação tem um nível de segurança e um propósito diferente.

Se alguém tentar fazer uma requisição para uma API sem enviar as informações de autenticação exigidas, o servidor irá recusar o request e responderá com um código de erro. Por isso, seja qual for o meio de autenticação escolhido, ele precisa estar especificado na documentação da API. Caso contrário, a pessoa que for desenvolver uma integração usando essa API não tem como saber quais informações ela precisa enviar para se autenticar.

## Composição de um request

Todo request é composto por elementos que, juntos, formam a solicitação que será feita para a API. Esses elementos podem variar para cada a API, mas suas especificações precisam ser seguidas para que a API processe a requisição com sucesso, caso contrário ela pode retornar um erro em vez da resposta esperada.

Estas são as partes que compõem um request para uma API do tipo REST:

* **Método:** é o tipo de operação da solicitação, como adicionar ou excluir um recurso, por exemplo.
* **URL da API:** é o endereço web onde a API está hospedada, ou seja, a URL para onde o protocolo HTTP deve direcionar a solicitação.
* **Path:** é o caminho onde o recurso se encontra na URL especificada acima.
* **Endpoint:** é nome do recurso que será acessado pela requisição.
* **Header:** é um bloco de informações adicionais sobre o request, como por exemplo informações sobre autenticação da API e o tipo de conteúdo que está sendo enviado.
* **Body:** é o bloco principal de informações, enviado junto com o Header. O Body contém o conteúdo que está sendo enviado na requisição, como os parâmetros para realizar uma consulta na API, ou um arquivo a ser armazenado, por exemplo.
* **Resposta:** é o retorno que a API devolve com base nos parâmetros indicados no Head e no Body.

As partes que compõem o request são definidas por quem desenvolveu a API. Para que o request funcione, a solicitação precisa respeitar todas as especificações da API. A melhor maneira de comunicar como a API funciona e quais dados ela espera num request, é por meio da **documentação dessa API**.

## Documentação de APIs

As partes que compõem um request são definidas por quem desenvolveu a API. Para que o request funcione, a solicitação precisa respeitar todas as especificações da API, estabelecidas durante o seu desenvolvimento, caso contrário irá retornar um erro em vez da resposta esperada.

APIs diferentes têm especificações diferentes de como esperam receber as requisições. Essas especificações têm diferentes níveis de complexidade e, quanto mais complexas forem, maior será a necessidade de que a API tenha uma documentação completa e clara.

A documentação de APIs é muito importante para que os desenvolvedores saibam como usar a API de forma eficaz e segura. Sem a documentação, desenvolvedores não têm como saber do que a API é capaz ou como usá-la.

### Exemplos reais

Para exemplificar a composição de um request e como ele pode ser descrito, vamos analisar alguns elementos de API na documentação de soluções reais do mercado.

A imagem abaixo foi tirada da [documentação do **Twilio**](https://www.twilio.com/docs). Ela mostra como o Twilio apresenta o **método**, a **URL**, o **PATH** e o **Endpoint** da requisição. Repare também como eles descrevem o objetivo da requisição, o que ela faz e o que ela retorna.

<p style="text-align: center; margin-top: 20px; margin-bottom: 20px;">
    <img src="/res/img/api-docs/conceito-03.png" alt-text="Exemplo de request na documentação do Twilio" title="Exemplo de request na documentação do Twilio" />
</p>

* **Método** = `POST`
* **URL** = `https://api.twilio.com`
* **Path/endpoint** = `/2010-04-01/Accounts.json`

Sobre a **autenticação**, o Twilio apresenta exemplos de comandos e descreve os tipos de autenticação aceitos. Além disso, a documentação também explica **onde e como** obter as credenciais necessárias.

<p style="text-align: center; margin-top: 20px; margin-bottom: 20px;">
    <img src="/res/img/api-docs/conceito-05.png" alt-text="Exemplo de request na documentação do Twilio" title="Exemplo de request na documentação do Twilio" />
</p>

Para as **respostas**, o Twilio descreve o que é retornado quando a requisição é feita com sucesso e lista os códigos de erro. Perceba na imagem abaixo como, além dos códigos, o Twilio explica a causa do erro e o que precisa ser verificado para resolver.

<p style="text-align: center; margin-top: 20px; margin-bottom: 20px;">
    <img src="/res/img/api-docs/conceito-04.png" alt-text="Exemplo de request na documentação do Twilio" title="Exemplo de request na documentação do Twilio" />
</p>

Por fim, a imagem abaixo mostra os **parâmetros do Body** de um request na [documentação de APIs do **Stripe**](https://stripe.com/docs). Ela lista, de duas maneiras diferentes, todos os parâmetros esperados pela API: uma **lista descritiva** com todos os atributos de cada parâmetro, e um **bloco de código** mostrando os mesmos parâmetros da forma como eles são estruturados dentro do protocolo HTTPS.

<p style="text-align: center; margin-top: 20px; margin-bottom: 20px;">
    <img src="/res/img/api-docs/conceito-06.png" alt-text="Exemplo de request na documentação do Twilio" title="Exemplo de request na documentação do Twilio" />
</p>

Como é possível notar, apesar de a documentação de APIs ter um padrão das informações que ela precisa ter, **não existe uma forma única de apresentá-las na documentação**. Existem diretrizes e boas práticas que direcionam a documentação para ser mais **útil** e **familiar** para desenvolvedores, mas você pode organizá-las de diferentes maneiras. Algumas das maneiras mais tradicionais de documentar APIs serão apresentadas ao longo deste tutorial, mas você pode usar a criatividade para criar e adaptar outras formas.

### OpenAPI Specification (OAS)

**OpenAPI Specification** (**OAS**) é uma linguagem usada para descrever e documentar APIs de forma padronizada.

A documentação no formato OAS contém informações sobre todos os componentes da API, como seus endpoints, parâmetros, métodos e respostas. Essas informações são armazenadas em um arquivo de forma estruturada, seguindo os padrões e normas da especificação. Normalmente, o arquivo de documentação seguindo a especificação OpenAPI tem os formatos **.JSON** ou **.YML**.

A vantagem de usar a especificação OAS é que ela pode ser lida por máquinas, o que significa que ela permite automatizar os processos de geração da documentação. Por seguir um padrão, o arquivo que segue essa especificação pode ser interpretado por diversas ferramentas e sistemas, facilitando a sua integração com o processo de desenvolvimento.

A especificação OAS é usada principalmente para construir **documentação de referência** das APIs, mas ela é capaz de comportar também **documentação conceitual**. (A diferença entre documentação de referência e conceitual está explicada no tópico sobre [Partes que compõem a documentação de APIs](/tutoriais/api-docs/partes-da-doc/).)

Você conhecerá um pouco mais sobre como usar arquivos OpenAPI na [seção sobre a ferramenta SwaggerHub](/tutoriais/api-docs/swaggerhub/) deste tutorial.

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/api-docs/postman/"><button type="button" class="btn btn-dark">Testando uma API com o Postman</button></a></p>
