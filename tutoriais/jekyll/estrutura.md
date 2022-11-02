---
layout: tutorial-jekyll
title: Tutorial | Jekyll - Estrutura de arquivos
permalink: /tutoriais/jekyll/estrutura/
---

# Estrutura de arquivos

O Jekyll usa uma estrutura de arquivos padronizada, com diretórios e arquivos que têm nomes e funções dinstintos.

Sempre que você cria um projeto novo, o Jekyll gera os arquivos básicos necessários para começar a trabalhar com o seu site.

Estes são alguns dos principais componentes da estrutura de arquivos:

<div class="alerta alerta-amarelo">
    <p>Alguns diretórios e arquivos mencionados a seguir só vão aparecer depois que você fizer o build do seu projeto pela primeira vez.</p>
</div>

<table class="table">
    <thead class="table-light">
        <tr>
            <th>Arquivos</th>
            <th>Descrição</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><b>config.yml</b></td>
            <td><p>Arquivo de configurações do Jekyll. Permite que você altere algumas propriedades e defina um padrão para algumas opções do projeto.</p><p>Inicialmente, deixe as configurações como foram criadas na instalação. Ao longo do tutorial você vai ver como fazer algumas das alterações necessárias.</p></td>
        </tr>
        <tr>
            <td><b>404.html</b></td>
            <td><p>Página com o conteúdo que será mostrado no navegador sempre que o usuário tentar acessar uma URL inexistente do seu site (o famoso erro <b>404 - Not found</b>). O arquivo já vem com uma mensagem de erro simples, mas você pode personalizar o conteúdo.</p></td>
        </tr>
        <tr>
            <td><b>about.markdown</b> e <b>index.markdown</b></td>
            <td><p>São duas páginas com conteúdo de exemplo, as quais o Jekyll cria automaticamente. O <b>index</b> sempre será a página inicial do seu site. É a primeira página que será exibida quando um usuário acessar o seu site no domínio raiz.</p></td>
        </tr>
        <tr>
            <td><b>Gemfile</b> e <b>Gemfile.lock</b></td>
            <td><p>O <b>Gemfile</b> contém informações sobre os Gems que você tem instalados no seu ambiente do Ruby, como as versões que você está usando, por exemplo.</p><p>O arquivo <b>Gemfile.lock</b> serve para bloquear alterações de novas instalações, a fim de evitar quebras de compatibilidade no seu projeto. Este bloqueio garante que você tenha controle sobre a atualização dos Gems.</p></td>
        </tr>
    </tbody>
</table>

<table class="table">
    <thead class="table-light">
        <tr>
            <th>Diretórios</th>
            <th>Descrição</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><b>_posts</b></td>
            <td><p>Se você usar o Jekyll para criar um blog, as páginas dos seus posts ficarão neste diretório.</p></td>
        </tr>
        <tr>
            <td><b>_site</b></td>
            <td><p>Este diretório é criado quando você fizer o primeiro build do seu projeto. Aqui ficam os arquivos gerados em cada build. O conteúdo do diretório <b>_site</b> contém o seu site gerado, incluindo os arquivos finais prontos para serem publicados.</p></td>
        </tr>
        <tr>
            <td><b>_layouts</b></td>
            <td><p>Este diretório agrupa os layouts que definem como será a estrutura das páginas do seu projeto. O diretório <b>_layouts</b> não é criado automaticamente em novos projetos do Jekyll; você irá criar este diretório manualmente durante uma das etapas do tutorial.</p></td>
        </tr>
    </tbody>
</table>

## Front Matter

O **Front Matter** é um conjunto de **atributos** e **valores** que servem para determinar características da sua página.

O Front Matter é a primeira coisa que você precisa inserir no seu arquivo.

O Jekyll interpreta os atributos inseridos no Front Matter e os aplica nas páginas geradas pelo build.

O Front Matter deve ter o seguinte formato:

````text
---
atributos: valores
---
````

Os **atributos** determinam características importantes da sua página.

O Jekyll tem diversos atributos e você pode definir quantos quiser.

Este tutorial usa dois dos atributos mais importantes:

* `title`: **título da página**. É o equivalente ao tag `<title>` de um HTML e é também o que vai aparecer no topo da janela do navegador.

* `layout`: **template da página**. Define o formato de estrutura que a página vai utilizar. Ao longo desse tutorial você vai ver como configurar o layout do jeito que quiser.

Você vai aprender a usar esses atributos nas próximas etapas do tutorial.

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/jekyll/criar-projeto/"><button type="button" class="btn btn-dark">Criar um projeto</button></a></p>
