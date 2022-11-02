---
layout: tutorial-jekyll
title: Tutorial | Jekyll - Publicar um projeto
permalink: /tutoriais/jekyll/publicar-projeto/
---

# Publicar um projeto

Esta seção do tutorial explica onde fica o site gerado pelo Jekyll e alguns aspectos sobre a publicação deste site.

## Localizar os arquivos do site

Sempre que você faz um build do seu projeto, o Jekyll compila todos os arquivos e gera um site estático.

Você pode localizar os arquivos do seu site gerado no diretório **_site**, dentro do diretório raiz do seu projeto.

No diretório **_site** fica armazenada a versão final dos arquivos, atualizada com suas novas alterações cada vez que você faz um build.

## Colocar o site no ar

Depois de criar todas as sus páginas e terminar o seu projeto, você pode publicar ele em algum lugar.

Uma das facilidades do Jekyll é que ele gera um site pronto sempre que você faz um **build** do projeto.

Depois do build, você só precisa localizar os arquivos gerados e colocá-los no local de hospedagem.

### Hospedagem do site

Assim como qualquer outro site, você precisa de um **serviço de hospedagem** para colocá-lo no ar.

Existem diversos serviços, tanto gratuitos quanto pagos, cada um com as suas vantagens e desvantagens.

O lado bom do Jekyll e dos sites considerados **estáticos**, é que eles não demandam nenhuma configuração especial da hospedagem. Eles podem ser executados praticamente em qualquer servidor, já que não há alterações no conteúdo durante a comunicação no [modelo cliente-servidor](https://pt.wikipedia.org/wiki/Modelo_cliente%E2%80%93servidor).

Depois de escolher o serviço de hospedagem, use o gerenciador de arquivos do próprio serviço ou um **cliente de FTP** para fazer o upload dos arquivos da pasta **_site**. Dessa forma, seu site estará no ar e pronto para ser acessado por qualquer pessoa.
