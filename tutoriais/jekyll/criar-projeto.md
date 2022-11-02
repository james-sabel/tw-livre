---
layout: tutorial-jekyll
title: Tutorial | Jekyll - Criar um projeto
permalink: /tutoriais/jekyll/criar-projeto/
---

# Criar um projeto

Esta seção do tutorial explica:

* como criar um projeto inicial com os arquivos essenciais do Jekyll
* como fazer um build (compilação) dos arquivos do seu projeto e abrir o site gerado
* como funcionam alguns recursos adicionais de projetos do Jekyll

## Criar um projeto inicial

1. Crie um diretório vazio no seu disco rígido. Esse diretório será o local onde o seu projeto ficará armazenado. Para este tutorial, considere o seguinte local de exemplo: **c:\projeto-tutorial**.

2. Acesse o terminal do **prompt de comando** do Windows. No terminal, navegue até o diretório que você criou no passo anterior.

3. Execute o comando `jekyll new` seguido do nome do seu projeto. Como o nome do projeto neste tutorial é **projeto-tutorial**, o comando ficará assim:
    ````
    jekyll new projeto-tutorial 
    ````
    {: .terminal }
    Este comando faz com que o Jekyll crie uma pasta onde serão instalados os [arquivos necessários](/tutoriais/jekyll/estrutura/) para o projeto inicial. Ao terminar a instalação do projeto, o prompt mostrará um aviso confirmando a criação da pasta.

## Fazer o build e abrir o site gerado

1. No **prompt de comando**, certifique-se de que você está posicionado no diretório onde seu projeto foi instalado. No exemplo deste tutorial, o local é este: **c:\projeto-tutorial\projeto-tutorial**.

2. Execute o seguinte comando para fazer um **build** do seu projeto:
    ````
    bundle exec jekyll serve
    ````
    {: .terminal }

3. Quando aparecer a mensagem indicando que o **build** foi finalizado, abra um navegador de sua preferência e acesse o seguinte endereço: **http://localhost:4000/**

Com isso você já poderá ver a versão inicial do seu site gerado.  

### Como funciona o build

No Jekyll você precisa compilar os arquivos do seu projeto para gerar os arquivos do site e visualizá-los no navegador. Este processo é chamado de **build**.

Sempre que você alterar um arquivo, é preciso fazer um novo build do projeto antes de visualizar a alteração.

Toda vez que você faz o build, os arquivos são disponibilizados em um servidor local da sua máquina.

### Tipos de build

Existem diferentes tipos de build. Estes são os mais comuns:

`bundle exec jekyll serve` ou `bundle exec jekyll s` — faz um build inicial do projeto e inicia o servidor local. Este tipo de build fica em constante execução, monitorando as alterações que você faz no seu projeto e atualizando os arquivos no output. Por padrão, o servidor local é iniciado na **porta 4000**.

`bundle exec jekyll serve --port 4001` — faz o mesmo que o tipo de build explicado acima, mas inicia o servidor em uma porta de sua escolha (substituindo o *4001*). Este tipo de build é especialmente útil quando você quer executar mais de um site ao mesmo tempo, rodando cada servidor em uma porta diferente.

`bundle exec jekyll serve --skip-initial-build` — apenas inicia o servidor local, sem fazer um build inicial do projeto.

<span class="nota azul">Sempre que você faz um build do seu projeto, todos os arquivos com extensão **.md** (Markdown) são convertidos para **.html** no output do seu site. Os arquivos originais do seu projeto permanecem com o formato **.md**.</span>

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/jekyll/editar-projeto/"><button type="button" class="btn btn-dark">Editar um projeto</button></a></p>
