---
layout: post
title: Bootstrap 4 Beta
---

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="//www.youtube.com/embed/aQUlA8Hcv4s?rel=0" width="760" height="570" allowfullscreen></iframe>
</div>

[Dois anos de fabricação](/2015/08/19/bootstrap-4-alpha/), finalmente temos nossa primeira versão beta do Bootstrap 4. Naquele tempo, quebramos todas as coisas, pelo menos, vinte e sete vezes, com quase 5.000 commits, 650+ arquivos mudados, 67.000 linhas adicionadas e 82.000 linhas foram excluídas. Nós também enviamos seis principais lançamentos alfa, um trio de Temas oficiais e até um quadro de trabalho para a boa medida. Simplificando? [Já estava na hora.](https://www.youtube.com/watch?v=_J6-3l3hCm0)
 

## Beta!?

Longa história curta, enviar uma versão beta significa que acabamos de romper todas as suas coisas até nossa próxima versão principal (v5). Nós não somos perfeitos, mas estaremos fazendo o nosso melhor para manter todas as classes, recursos e URL docs como aparecem agora neste lançamento. Nós sempre podemos adicionar mais coisas, mas não podemos tirar.

Para aqueles que não estiveram usando os lançamentos alfa v4, aqui estão alguns destaques para ajudar você.

- **Mudou-se de Less para Sass.** O Bootstrap agora compila mais rápido do que nunca graças ao Libsass, e nos juntamos a uma comunidade cada vez maior de desenvolvedores da Sass.
- **Flexbox e um sistema de grade melhorado.** Mudamos quase tudo para a flexbox, adicionamos um novo nível de grade para melhor segmentar dispositivos móveis e revisamos completamente nossa fonte Sass com melhores variáveis, mixins e agora mapas.
- **Dropped wells, thumbnails e panels para cards.** Os [Cards](https://getbootstrap.com/docs/4.0/components/card/) são um novo componente para o Bootstrap, mas eles se sentirão super familiares, como eles fazem quase tudo bem, thumbnails e panels fez, só que melhor.
- **Forked Normalize.css e consolidou todas as nossas restaurações de HTML em um novo módulo CSS, Reboot.** O Normalize.css tomou um caminho diferente do que preferiria, deixando alguns ajustes básicos do CSS que há muito dependemos. O Reboot leva o núcleo do Normalize.css e o expande para incluir retornos mais opcionais, como `box-sizing: border-box`, ajustes de margem e mais tudo em um único arquivo Sass.
- **Novas opções de personalização.** Em vez de relegar enfeites de estilo como gradientes, transições, sombras, classes de grade e mais para uma folha de estilos separada, como a v3, movemos todas essas opções para variáveis Sass. Deseja transições padrão em tudo ou para desativar cantos arredondados? Basta atualizar uma variável e recompilar.
- **Abandonou o suporte IE8 e IE9**, caiu versões mais antigas do navegador, e se mudou para unidades rem para o dimensionamento componente para aproveitar o suporte CSS mais recente. Além da nossa grade, os pixels foram trocados para rems e ems, quando apropriado, para tornar a tipografia responsiva e o dimensionamento de componentes ainda mais fácil. Precisa de suporte para IE8 / IE9, Safari 8-, iOS 8-, etc? Continue usando o Bootstrap 3.
- **Reescreveu todos os nossos plugins de JavaScript.** Cada plugin foi reescrito no ES6 para tirar proveito dos mais recentes aprimoramentos de JavaScript com novos métodos de desmontagem, verificação de tipo de opção, novos métodos e muito mais.
- **Melhoria da auto-colocação de tooltips, popovers, e menus suspensos** graças à ajuda de uma biblioteca chamada [Popper.js](https://popper.js.org).
- **Documentação redigada e melhorada.** Nós redesenhamos, reescrevemos tudo no Markdown e adicionamos alguns plugins acessíveis para simplificar exemplos e trechos de código para facilitar o trabalho com nossos documentos. Nós também adicionamos um incrível novo formulário de pesquisa!
- **Novas ferramentas** de compilação completamente reescritas em scripts npm em vez de Grunt, imensamente simplificando o processo de desenvolvimento e contribuição para o Bootstrap.
- **E muito mais!** Controles de formulário personalizados, um carrossel redesenhado, uma barra de navegação revisada, estilos de validação de formulário HTML5, centenas de classes de utilidade responsivas, novos componentes e muito mais também foram incluídos.

Ok, então, quer aprender ainda mais? Continue lendo ou vá diretamente para [esses novos documentos](https://getbootstrap.com)!

## Novo Visual
O Bootstrap 4 tem um aspecto levemente atualizado ao longo de nossas versões alfa, mas não foi até recentemente que nós demos os documentos e os nossos componentes também se refrescaram.

[![Bootstrap 4 beta docs](/img/2017/bootstrap-4-beta.png)](https://getbootstrap.com)

Além de uma nova paleta de cores e fontes de novos sistemas, temos um novo layout para nossa documentação. Novo com este beta é um incrível formulário de pesquisa alimentado pela [DocSearch](https://community.algolia.com/docsearch/) da Algolia, um layout de página melhorado com barra lateral e barra lateral e um novo índice.

---

For more details on this release's changes, take a look at the [Beta 1 ship list issue](https://github.com/twbs/bootstrap/issues/21568), as well as the [closed Beta 1 milestone](https://github.com/twbs/bootstrap/milestone/41?closed=1). Be sure to [join our official Slack room!](https://bootstrap-slack.herokuapp.com) and dive into [our issue tracker](https://github.com/twbs/bootstrap/issues/) with bug reports, questions, and general feedback whenever possible.

<3,<br>
[@mdo](https://twitter.com/mdo) & [team](https://github.com/twbs)

Tradução: [@haynes](http://haynes.blog.br)
