---
layout: tutorial-github
title: Tutorial | GitHub e open source - Enviar uma contribuição
permalink: /tutoriais/github/enviar-contribuicao/
---

# Enviar uma contribuição

<div class="alerta alerta-azul">
    <p>Este tópico usa vários termos relacionados ao GitHub e a controle de versão. Se você não está familiarizado com os termos usados aqui, acesse os tópicos anteriores deste tutorial.</p>
</div>

Estas são as etapas que você normalmente deve seguir para enviar uma contribuição para um projeto pelo GitHub:

<table style="margin-top: 15px; margin-bottom:15px;padding: 5px;">
    <tr>
        <td style="padding: 5px 15px 5px 15px; background-color: #333333; color: #fff;">1</td>
        <td style="padding: 5px; background-color: #dedede;"><b>Fork</b> do projeto original (aquele com que você quer contribuir)</td>
    </tr>
    <tr>
        <td style="padding: 5px 15px 5px 15px; background-color: #333333; color: #fff;">2</td>
        <td style="padding: 5px; background-color: #cecece;"><b>Clone</b> do projeto originado pelo fork</td>
    </tr>
    <tr>
        <td style="padding: 5px 15px 5px 15px; background-color: #333333; color: #fff;">3</td>
        <td style="padding: 5px; background-color: #dedede;">Alterar o projeto <b>localmente</b></td>
    </tr>
    <tr>
        <td style="padding: 5px 15px 5px 15px; background-color: #333333; color: #fff;">4</td>
        <td style="padding: 5px; background-color: #cecece;"><b>Stage</b> dos arquivos alterados</td>
    </tr>
    <tr>
        <td style="padding: 5px 15px 5px 15px; background-color: #333333; color: #fff;">5</td>
        <td style="padding: 5px; background-color: #dedede;"><b>Commit</b> dos arquivos alterados</td>
    </tr>
    <tr>
        <td style="padding: 5px 15px 5px 15px; background-color: #333333; color: #fff;">6</td>
        <td style="padding: 5px; background-color: #cecece;"><b>Push</b> dos arquivos alterados</td>
    </tr>
    <tr>
        <td style="padding: 5px 15px 5px 15px; background-color: #333333; color: #fff;">7</td>
        <td style="padding: 5px; background-color: #dedede;"><b>Pull request</b> das alterações</td>
    </tr>
    <tr>
        <td style="padding: 5px 15px 5px 15px; background-color: #333333; color: #fff;">8</td>
        <td style="padding: 5px; background-color: #cecece;">Aguardar análise do pull request</td>
    </tr>
</table>

Quer mais detalhes de cada etapa? Confira o passo a passo na seção a seguir.

## Passo a passo

Suponha que você quer contribuir com o projeto do **TW Livre** no GitHub. Isto é o que você precisa fazer:

1. Faça o **fork** do [projeto TW Livre](https://github.com/james-sabel/tw-livre). Isto vai fazer uma cópia do projeto para a sua própria conta do GitHub.
2. Acesse o projeto do GitHub na **sua** conta do GitHub (obtido pelo **fork**) e faça o **clone** do repositório. Isto vai criar uma **cópia local** do projeto.
3. Abra o projeto na sua cópia local e altere os arquivos como quiser. Pode ser uma correção, melhoria ou criação de novo conteúdo ou no site. Ao fazer qualquer alteração, os arquivos alterados ficarão com o status **Add**.
4. Quando achar que as alterações estão prontas, faça um **Stage** dos arquivos alterados.
5. Certifique-se de que as alterações estão concluídas e faça um **Commit**, indicando que você está pronto para enviá-las para a **cópia remota** do projeto.
6. Faça um **Push** dos arquivos. Isto envia todas as alterações para a **cópia remota** na sua própria conta do GitHub.
7. No GitHub, faça um **pull request** das alterações que você acabou de enviar pelo **push**. O **pull request** vai enviar as alterações que você fez no projeto da sua conta para o repositório da conta de origem (neste caso, o projeto original do TW Livre).
8. A pessoa responsável pelo repositório de origem recebe o seu **pull request** e analisa as alterações. Aqui, essa pessoa normalmente toma *uma* das seguintes ações:
    * Ela decide que suas alterações estão **corretas** e são válidas. Então, ela faz o **merge** das alterações, incorporando-as ao projeto de origem.
    * Decide que suas alterações **precisam de ajustes** e sugere as correções. Então, você faz os ajustes e envia um novo **pull request**, que volta para o ciclo de aprovação.

**Pronto! \o/** Você acabou de fazer a sua primeira contribuição em um projeto open-source.