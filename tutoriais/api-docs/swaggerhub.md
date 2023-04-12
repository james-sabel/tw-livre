---
layout: tutorial-api-docs
title: Tutorial | Documentação de APIs - SwaggerHub
permalink: /tutoriais/api-docs/swaggerhub/
---

# SwaggerHub

Nesta parte do tutorial você vai conhecer a ferramenta **SwaggerHub** e aprender a usá-la para gerar uma documentação de forma automática a partir de um arquivo na especificação OpenAPI (OAS).

## Sobre o SwaggerHub

O SwaggerHub é uma ferramenta para documentar APIs do tipo REST a partir de arquivos que seguem a especificação OpenAPI. Esta ferramenta é muito popular no desenvolvimento de software, devido à facilidade e simplicidade para gerar a documentação.

Você pode conferir o resultado que pode ser obtido com o SwaggerHub na [página de demonstração da ferramenta](https://petstore.swagger.io/).

O projeto Swagger ficou conhecido pela automação de documentação de APIs. Inclusive, antes da especificação OAS receber esse nome, essa especificação era conhecida apenas como *Swagger*. Por isso, até hoje você ainda vai ouvir pessoas chamando o arquivo de especificação OpenAPI de *Swagger*, apesar de este não ser o nome atual da especificação. A verdade é que a especificação OAS teve diferentes versões, sendo que o Swagger era a versão 2.0. Depois de ter se transformado num formato aberto, a especificação Swagger foi modificada e deu origem à versão 3.0, que passou a se chamar OpenAPI.

O SwaggerHub é apenas uma das muitas ferramentas que interpretam arquivos que seguem a especificação OpenAPI. O SwaggerHub foi escolhido para este tutorial pela sua popularidade, mas existem diversas opções no mercado.

## Gerando documentação usando o SwaggerHub

### Antes de começar

* Crie uma conta gratuita no site da ferramenta: [https://swagger.io/](https://swagger.io/)

### Importando o arquivo de especificação OpenAPI no SwaggerHub

1. Acesse a [aplicação do SwaggerHub](https://app.swaggerhub.com/) e faça login com a sua conta.
2. No menu lateral, clique em **Create New** e depois em **Import and Document API**.
    * Com esta opção, você importará o arquivo de especificação da API diretamente de uma URL onde ele está hospedado. Mas o SwaggerHub também permite que você importe arquivos locais ou criar um arquivo diretamente na plataforma.

    <img src="/res/img/api-docs/tutorial-swaggerhub-01.png" alt-text="Botão para importar um arquivo de especificação OpenAPI" title="Botão para importar um arquivo de especificação OpenAPI" class="imagem-curso" />

3. Coloque a seguinte URL no campo **Path or URL**: `https://www.twlivre.org/tutoriais/api-docs/twlivre-sunrise-sunset-api.yml`
    * Este caminho direciona para um arquivo de especificação da API de consulta de horário solar (a mesma API que construímos no [tutorial de Postman](/tutoriais/api-docs/postman/)).
4. Selecione seu nome em **Owner** e mantenha o campo **Visibility** como **Public**.
   * Só é possível manter documentações públicas na versão gratuita do SwaggerHub, mas você pode criar uma conta paga ou de uma organização para ter acesso ao recurso de documentações privadas.
5. Clique em **Upload file**. Nesse momento, o SwaggerHub irá validar a estrutura do arquivo de especificação.

    <img src="/res/img/api-docs/tutorial-swaggerhub-02.png" alt-text="Tela para importar um arquivo de especificação OpenAPI" title="Tela para importar um arquivo de especificação OpenAPI" class="imagem-curso" />

6. Depois da validação, informe um nome para a API e clique em **Import definition** para concluir a importação. Nesse momento, o SwaggerHub irá apresentar uma tela dividida em dois painéis: um com o código-fonte do arquivo que acabamos de importar e outro com a visualização da documentação do arquivo, já interpretada pelo SwaggerHub.

    <img src="/res/img/api-docs/tutorial-swaggerhub-03.png" alt-text="Tela apresentando o arquivo OAS editável e a prévia da documentação gerada" title="Tela apresentando o arquivo OAS editável e a prévia da documentação gerada" class="imagem-curso" />

7. Clique no botão **View documentation** para abrir a documentação gerada com base no arquivo que você importou.

    <img src="/res/img/api-docs/tutorial-swaggerhub-04.png" alt-text="Botão para abrir a documentação gerada a partir da especificação OpenAPI" title="Botão para abrir a documentação gerada a partir da especificação OpenAPI" class="imagem-curso" />

## SwaggerHub - considerações finais

Como dito anteriormente, o SwaggerHub é apenas uma das várias [ferramentas](/tutoriais/api-docs/ferramentas/) que interpretam arquivos de especificação OpenAPI. Cada ferramenta tem limitações e recursos diferentes, com níveis distintos de personalização e algumas até permitem criar portais inteiros para desenvolveores, misturando documentação conceitual com documentação de referência.
