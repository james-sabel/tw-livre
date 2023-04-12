---
layout: tutorial-api-docs
title: Tutorial | Documentação de APIs - Testando uma API com o Postman
permalink: /tutoriais/api-docs/postman/
---

# Testando uma API com o Postman

Esta parte do tutorial fala sobre:

* o que são testes de API e sua importância
* como testar uma API na prática usando a plataforma Postman

## Teste de APIs

Testar uma API significa fazer requests para a aplicação e consumir as respostas dessas requisições.

Os testes de API têm diversas finalidades:

* Para o time que desenvolve a API, incluindo desenvolvedores e profissionais de testes:
  * testar se a API está funcionando corretamente
  * identificar possíveis melhorias na arquitetura da API
* Para o lado do cliente, que desenvolve a aplicação que consome os dados da API:
  * verificar se os requests foram construídos corretamente
  * verificar se as respostas contém os dados esperados e como estão estruturadas

Existem várias maneiras de testar uma API. Uma delas é usando plataformas chamadas de **API clients**, ou clientes de API.

Para este tutorial vamos usar o **Postman**, um dos API clients mais populares.

## Postman

### Acessando o Postman

O Postman está disponível via **instalação local** e em **versão web**. Vamos usar a versão web neste tutorial, mas você pode fazer as mesmas operações usando a instalação local.

* **Instalação local:** acesse o [site do Postman](https://www.postman.com/), faça o download do aplicativo e instale no seu sistema.
* **Versão web:** acesse a [versão web do Postman](https://web.postman.co/) para usá-la no seu navegador.
  * A versão web exige que você crie uma conta no Postman. A criação de uma conta é gratuita e oferece algumas facilidades adicionais, como sincronizar entre dispositivos as suas configurações, preferências e definições de APIs que você usa com frequência.

### Fazendo requests para uma API sem parâmetros

Para o primeiro teste prático com o Postman, vamos usar uma **API que retorna citações de Ron Swanson**. (Ron Swanson é um dos personagens da série de TV "Parks and Recreation", conhecida no Brasil como "Parks & Recreation: Confusões de Leslie".)

A API de citações do Ron Swanson é uma API gratuita que está disponível para qualquer pessoa enviar requisições livremente.

Esta é uma API simples porque ela não exige nenhuma informação especial para a requisição. Não é preciso fazer nenhum tipo de autenticação e nem enviar dados no Header ou Body. Basta você fazer um request para a URL da API e ela já retorna os dados solicitados, neste caso, uma citação do Ron Swanson.

**Passos para fazer a requisição:**

1. Acesse o Postman na web ou na sua instalação local.
1. No menu lateral esquerdo, acesse a seção **Collections** e clique no ícone para adicionar uma nova coleção
    * Coleções do Postman são uma forma de organizar as definições de APIs. É comum que Tech Writers tenham que lidar com diferentes APIs no dia a dia. As coleções permitem agrupar as configurações de requests dessas APIs, facilitando os testes e a operação com cada uma.
    <img src="/res/img/api-docs/tutorial-postman-01.png" alt-text="Botão para criar uma nova coleção" title="Botão para criar uma nova coleção" class="imagem-curso" />
1. Renomeie a coleção para "Citações do Ron" para ficar mais fácil de identificá-la. Em seguida, clique em **Add a request** para incluir uma nova requisição nessa coleção.   
    <img src="/res/img/api-docs/tutorial-postman-02.png" alt-text="Renomeando a coleção e adicionando um novo request" title="Renomeando a coleção e adicionando um novo request" class="imagem-curso" />
1. Renomeie o request para **Buscar uma citação aleatória**.
    * Note que o nome descreve exatamente o que o request faz: ele busca, aleatoriamente, uma citação do personagem em uma base de dados onde tem uma extensa lista de citações.
    * É uma boa prática que os nomes de requests usem *verbos* para indicar uma *ação*.
1. Mantenha o método **GET** preenchido. Você poderia escolher qualquer outro método, mas esta API aceita apenas o método GET, pois ela permite apenas *buscar* um recurso da API.
1. Preencha a URL da requisição logo ao lado do método. A URL da requisição da API de citações do Ron Swanson é a seguinte:
    * `https://ron-swanson-quotes.herokuapp.com/v2/quotes`
    * Sua tela do Postman deve se parecer com a imagem abaixo:
    <img src="/res/img/api-docs/tutorial-postman-03.png" alt-text="Request renomeado, método GET selecionado e URL preenchida" title="Request renomeado, método GET selecionado e URL preenchida" class="imagem-curso" />
2. Clique em **Send** para enviar a sua requisição e pronto! Na área inferior você pode conferir a resposta da requisição, onde aparece uma citação aleatória do Ron.
    <img src="/res/img/api-docs/tutorial-postman-04.png" alt-text="Resposta retornada pela requisição" title="Resposta retornada pela requisição" class="imagem-curso" />
3. Clique em **Send** novamente e perceba que você receberá uma nova resposta da API, com uma nova citação aleatória. Cada vez que você enviar uma requisição, a API responderá com uma citação diferente.

<p style="text-align: center;">
    <img src="/res/img/api-docs/ron-swanson-done.gif" alt-text="GIF animado do personagem Ron Swanson falando Done and Done" title="O personagem Ron Swanson falando Done and Done" style="max-height: 300px" />
</p>

<div class="alerta alerta-azul">
    <p>Algumas APIs podem estabelecer um <b>limite de requisições</b>. Cada requisição consome recursos da API, então é normal que algumas empresas permitam fazer apenas um número máximo de requisições e, depois de atingir o limite, comecem a cobrar por cada requisição realizada. Mas não se preocupe: este não é o caso da API de citações do Ron Swanson!</p>
</div>

### Fazendo requests para uma API com parâmetros

Para o segundo teste prático com o Postman, vamos usar a **API Sunset and Sunrise Times**. Ela traz os horários do nascer do sol e do pôr do sol em um determinado local.

O Sunset and Sunrise Times é uma API gratuita que está disponível para qualquer pessoa enviar requisições livremente.

Esta é uma API que exige que você informe alguns parâmetros na requisição, para que o serviço saiba o lugar para o qual você quer consultar os horários solares. A consulta é feita com base na **latitude** e **longitude** informadas na requisição. Esses parâmetros são obrigatórios, mas a API aceita alguns parâmetros adicionais que são opcionais.

<div class="alerta alerta-azul">
    <p>A API Sunset and Sunrise Times é de propriedade do site <a href="https://sunrise-sunset.org/" target="_blank">Sunrise-Sunset.org</a> e oferecida livremente na internet.</p>
</div>

**Passos para fazer a requisição:**

1. Acesse o Postman na web ou na sua instalação local.
2. No menu lateral, acesse a seção **Collections** e clique no ícone para adicionar uma nova coleção
3. Renomeie a coleção para "Horário solar" para ficar mais fácil de identificá-la. Em seguida, clique em **Add a request** para incluir uma nova requisição nessa coleção.
4. Renomeie o request para **Buscar horário solar de um local**.
5. Mantenha o método **GET** preenchido. Esta API aceita apenas o método GET, pois ela permite apenas *buscar* um recurso da API.
6. Preencha a URL da requisição logo ao lado do método. A URL de requisição desta API é a seguinte:
    * `https://api.sunrise-sunset.org/json`
7. Clique na guia **Params** e preencha as colunas **Key**, **Value** e **Description** dos parâmetros com os valores abaixo:
    * Parâmetro 1:
        * **Key** = lat
        * **Value** = 36.7201600
        * **Description** = Latitude
    * Parâmetro 2:
        * **Key** = lng
        * **Value** = 4.4203400
        * **Description** = Longitude
    * Sua tela do Postman deve se parecer com a imagem abaixo:
    <img src="/res/img/api-docs/tutorial-postman-05.png" alt-text="Request renomeado, método GET selecionado, URL preenchida e parâmetros cadastrados" title="Request renomeado, método GET selecionado, URL preenchida e parâmetros cadastrados" class="imagem-curso" />
8. Clique em **Send** para enviar a sua requisição e pronto! Na área inferior você pode conferir a resposta da requisição, onde aparecem as informações de horário solar para as coordenadas informadas nos parâmetros.
    <img src="/res/img/api-docs/tutorial-postman-06.png" alt-text="Resposta retornada para a data atual (comportamento padrão)" title="Resposta retornada para a data atual (comportamento padrão)" class="imagem-curso" />

Perceba que o teste acima não especifica de **quando** são os horários solares retornados. A API tem um comportamento padrão que é considerar sempre a **data atual**, caso você não informe a data de quando quer consultar. Vamos fazer um novo teste colocando uma data como parâmetro:

1. Acesse o request **Buscar horário solar de um local** que você criou nos passos anteriores.
2. Abaixo do parâmetro de longitude, adicione um novo parâmetro:
    * **Key** = date
    * **Value** = tomorrow
    * **Description** = Data
3. Clique em **Send** para enviar a sua requisição. Agora, na área inferior você pode conferir a resposta da requisição, onde aparecem as informações de horário solar para as coordenadas informadas nos parâmetros.
    <img src="/res/img/api-docs/tutorial-postman-07.png" alt-text="Resposta retornada para a data especificada no parâmetro" title="Resposta retornada para a data especificada no parâmetro" class="imagem-curso" />

Experimente fazer novas consultas trocando as coordenadas e a data. Você pode consultar os horários solares de qualquer lugar e para qualquer data que quiser.

Para conhecer todas as opções de parâmetros que você pode usar, consulte a [documentação oficial da API Sunset and Sunrise Times](https://sunrise-sunset.org/api). Perceba como até mesmo uma API simples como essa precisa de documentação!

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/api-docs/ferramentas/"><button type="button" class="btn btn-dark">Ferramentas para documentar APIs</button></a></p>
