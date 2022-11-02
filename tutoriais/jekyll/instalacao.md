---
layout: tutorial-jekyll
title: Tutorial | Jekyll - Instalação
permalink: /tutoriais/jekyll/instalacao/
---

# Instalação

Esta documentação explica como instalar o Ruby, o Jekyll e o Bundler. Depois de seguir estas orientações, seu ambiente estará pronto para criar e editar projetos usando o Jekyll.

---

## Baixe e instale o RubyInstaller

1. [Clique aqui](https://rubyinstaller.org/downloads/){:target="_blank"} para acessar a página de download do **RubyInstaller** para Windows.
   
2. Faça o download do arquivo de instalação. Escolha a versão recomendada na própria página de download, apenas certifique-se que seja uma versão **com o DevKit** (*RubyInstaller with DevKit*).
   
3. Aguarde até o download terminar e execute o instalador. Siga os passos do instalador sem alterar nenhuma das opções de instalação padrão.
    <div class="alerta alerta-vermelho">
    <p>Na última etapa da instalação, você vai ver a opção <b>Run ‘ridk install’ to setup MSYS2 and development toolchain</b>. Mantenha esta opção <b>selecionada</b>.</p>
    </div>

4. Clique em **Finish**. Uma tela de terminal será aberta automaticamente, pedindo para escolher uma das opções do **ridk install**. Simplesmente tecle <span class="tecla">Enter</span> para fazer a instalação padrão.

5. Aguarde até o **ridk install** terminar e feche a janela do terminal.

Se tudo foi feito corretamente, agora você tem o **Ruby** instalado na sua máquina.

## Instale o Jekyll e o Bundler

1. Acesse o terminal do **prompt de comando** do Windows.
   
2. Execute o comando abaixo na tela do terminal. Este comando inicia a instalação do **Jekyll** e do **Bundler**:\
`gem install jekyll bundler`

3. Aguarde até o final da instalação dos pacotes e verifique se o **Jekyll** foi instalado corretamente.<br>Para verificar a instalação, ainda na janela do terminal, execute o comando abaixo:\
`jekyll -v`

Se o terminal retornar a versão do Jekyll (exemplo: `jekyll 4.2.0`) é porque deu tudo certo.

**Pronto!** Agora você tem tudo que você precisa para começar a usar o Jekyll.

---

<p class="proxima-unidade"><b>Próximo:</b> <a href="/tutoriais/jekyll/estrutura/"><button type="button" class="btn btn-dark">Estrutura de arquivos</button></a></p>
