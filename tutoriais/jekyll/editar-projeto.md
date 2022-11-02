---
layout: tutorial-jekyll
title: Tutorial | Jekyll - Editar um projeto
permalink: /tutoriais/jekyll/editar-projeto/
---

# Editar um projeto

Esta seção do tutorial explica:

* os primeiros passos para começar a editar um projeto inicial do Jekyll
* algumas técnicas básicas para entender como funcionam o Front Matter e os layouts do Jekyll

## Editar a página inicial

1. Use uma ferramenta de edição de texto e código da sua escolha para abrir o arquivo **index.markdown**. Este é um dos arquivos que foram gerados automaticamente pelo Jekyll quando você criou o seu projeto inicial.

2. Apague todo o conteúdo do arquivo e substitua pelo seguinte Front Matter:

    ```text
    ---
    layout: geral
    title: Página inicial
    ---
    
    # Olá, mundo!
    
    Esta é a minha primeira página.
    ```

    Com isso, você terá criado sua primeira página e definido que ela irá usar um layout chamado **geral**. Este layout ainda não existe, então vamos criá-lo agora.

3. Crie um diretório chamado **_layouts** dentro do diretório raiz do seu projeto. Por padrão, este é o nome do local onde o Jekyll busca os layouts do projeto.

4. Crie um arquivo chamado **geral.html** dentro do diretório **_layouts**.

5. Abra o arquivo **geral.html** usando o seu editor de preferência e faça as seguintes alterações:

    * Adicione o parâmetro {% raw %}`{{ page.title }}`{% endraw %} dentro do tag de título da página. Na saída gerada pelo build do seu projeto, o parâmetro {% raw %}`{{ page.title }}`{% endraw %} é substituído automaticamente pelo **título** da página que o usuário estiver acessando.
    * Adicione o parâmetro {% raw %}`{{ content }}`{% endraw %} entre os tags `<body> </body>`. Na saída gerada pelo build do seu projeto, o parâmetro {% raw %}`{{ content }}`{% endraw %} é substituído automaticamente pelo **conteúdo** (corpo) da página que o usuário estiver acessando.

      Depois de fazer estas alterações, o conteúdo do arquivo **geral.html** deverá estar assim:

      ```html
      <!doctype html>
      <html>
      <head>
      <meta charset="utf-8">
      <title>{% raw %}{{ page.title }}{% endraw %}</title>
      </head>
      <body>
          {% raw %}{{ content }}{% endraw %}
      </body>
      </html>
      ```

6. Faça o build do projeto, caso não tenha o feito. Com o servidor local do Jekyll em execução, acesse o seguinte endereço no seu navegador: [http://localhost:4000](http://localhost:4000)

    Ao acessar o endereço, você verá a página inicial que você criou. A página deverá mostrar o seguinte conteúdo:

    ```text
    Olá, mundo!

    Esta é a minha primeira página.
    ```

## Criar uma nova página e fazer links

1. Crie um arquivo chamado **pagina2.md** dentro do diretório raiz do seu projeto. Abra o arquivo no seu editor de preferência e coloque o seguinte conteúdo:

    ```text
    ---
    layout: geral
    title: Página 2
    ---

    # Oi! Sou eu de novo.

    Esta é a segunda parte do meu site.
    ---
    ```

    Perceba que, assim como a página inicial que criamos, esta aqui também usa o layout **geral**. Mas, se você quisesse, poderia criar um layout diferente e defini-lo aqui.

2. Abra o arquivo **index.markdown**. Você deverá criar um link dele para a página **pagina2.md** que você acabou de criar. Para criar o link, acrescente mais uma linha no final do arquivo **index.markdown**, como demonstrado a seguir:

    ```text
    ---
    layout: geral
    title: Página inicial
    ---
    
    # Olá, mundo!
    
    Esta é a minha primeira página.

    Mas eu também tenho [mais uma página](pagina2.md).
    ```

    Ao fazer isso, você linkou o texto **mais uma página** com a página do arquivo **pagina2.md**.

3. Faça o build do projeto, caso não tenha o feito. Com o servidor local do Jekyll em execução, acesse o seguinte endereço no seu navegador: [http://localhost:4000](http://localhost:4000)

4. Clique no link que você acabou de criar e veja que, assim, você navegou da página inicial para a segunda página do seu projeto. É desse jeito que você cria links entre páginas escrevendo em Markdown e no Jekyll.

## Temas do Jekyll e personalização

Os projetos criados com o Jekyll suportam o uso de **temas**.

Temas são templates que determinam a aparência de todo o projeto. Por padrão, a instalação de um novo projeto do Jekyll usa um tema básico chamado **Minima**.

Este tutorial não explica como editar seu projeto usando temas personalizados. Mas, para personalizar o seu projeto, você pode pesquisar por temas do Jekyll na internet. Existem temas pagos e gratuitos.

Se você conhece **CSS**, ele também é uma alternativa para customizar a aparência do seu site. O Jekyll suporta totalmente esta linguagem, assim como outras linguagens web.

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/jekyll/publicar-projeto/"><button type="button" class="btn btn-dark">Publicar um projeto</button></a></p>
