---
layout: post
title: Novo Bootstrap 4 alpha
---

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" width="648" height="365" src="https://www.youtube.com/embed/J_kokTee01k" frameborder="0" allowfullscreen></iframe>
</div>

Bootstrap 4 alpha 2 já está disponível. Desde nossa última versão, quase 100 pessoas fizeram envios em mais de 900 commits para a v4 e nós fechamos mais de 400 issues e pull requests. Esses números são exorbitantemente impressionantes de se ver, e ainda temos uma tonelada de trabalho pela frente neste ano para a v4.

Como mensionado em nosso último post, o plano geral de desenvolvimento da v4 começa com uns poucos lançamentos alpha. Nós estamos um pouco atrás nisso, mas deve ser recuperado conforme os ventos do ano cairem. Espere um alpha ou dois neste mês para realmente ser lançado.

Aqui está um pouco das mudanças desde nosso último alpha:

- Revisado espaçamento de utilitários para usar uma hierarquização numérica (para evitar confusão com camadas de grids).
- Continuado esforços de refatoramento para substituir seletores de marcações específicas com classes através de vários componentes (includindo paginação, listas, e mais). *Ainda mais para fazer aqui com componentes adicionais*.
- Reverter media queries e containers de grid de rems para pixels porque viewports não são afetadas por font-size. Veja [#17403](https://github.com/twbs/bootstrap/pull/17403) para detalhes. *Nós temos uma tonelada de trabalho de grid, também. Sinta-se livre para seguir junto com [#18471](https://github.com/twbs/bootstrap/issues/18471)*.
- Revertido <code>.0625rem</code> com bordas para <code>1px</code> para maior consistência de  bordas de componentes que evitam zoom e bugs de font-size entre os navegadores.
- Renomeado <code>.img-responsive</code> para <code>.img-fluid</code> para evitar futuras confusões nas várias soluções de imagem responsiva fora essas.
- Substituído ZeroClipboard com clipboard.js para a cópia botões independente em Flash.
- Entradas e botões atualmente compartilham a mesma variável de borda para assegurar que os componentes tenham sempre tamanhos similares.
- Atualizados todos os seletores pseudo-elementos para usar as especificações preferidas de duplo dois pontos (ex.:, <code>::before</code> como oposto para <code>:before</code>).
- Cartões agora têm variação de contorno e mixins para apoiar extenções de classes base adicionais.
- Classes utilitárias para para floats e alinhamento de texto agora tem variações responsivas. *Isso significa que nós temos largado as classes não responsivas para evitar duplicação*.
- Adicionado suporte para jQuery 2.
- E mais centenas de melhorias Sass, correções de bugs, atualização da documentação, e mais.

Nós altamente encorajamos pessoas a folhear através da [segunda milestone no GitHub](https://github.com/twbs/bootstrap/issues?q=milestone%3Av4.0.0-alpha.2+is%3Aclosed) para uma ideia melhor do que foi mudado sobre o projeto. Você pode também seguir junto com outros esforços da v4 com a [etiqueta <code>v4</code>](https://github.com/twbs/bootstrap/labels/v4) em nossa rastreadora de issue.

Pronto pra mergulhar? Então, [caia de cabeça na documentação aplha v4](http://getbootstrap.com.br/v4-alpha/)!

Certifique-se de juntar-se a [nossa sala oficial no Slack](https://bootstrap-slack.herokuapp.com/)! e mergulhe em [nossa rastreadora de issue](https://github.com/twbs/bootstrap/issues/) com relatório de bugs, questões, e comentários geral sempre que possivel.

<3,

[@mdo](https://twitter.com/mdo), [@fat](https://twitter.com/fat), & [team](https://github.com/twbs)

Tradução: [@flaviacs](https://github.com/flaviacs)