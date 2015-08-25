---
layout: post
title: Bootstrap 4 alpha
---

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="//www.youtube.com/embed/4PdU6migsqQ?rel=0" width="760" height="570" allowfullscreen></iframe>
</div>

Hoje é um dia especial para Bootstrap. Não só pelo nosso [quarto aniversário](https://twitter.com/mdo/statuses/104620039650557952), como também, depois de um ano de desenvolvimento, estamos finalmente divulgando a primeira versão alpha do Bootstrap 4. É isso aí!

Bootstrap 4 tem sido uma grande empreendimento que altera quase todas as linhas de código. Estamos felizes por compartilhar com você e ouvir seus comentários. Nós temos um monte de notícias para compartilhar com você, então vamos pular direto para elas.

## O que há de novo

[![Bootstrap 4 alpha](http://bootstrapbrasil.github.io/bootstrap-blog/img/2015/bs4-alpha.png)](http://v4-alpha.getbootstrap.com)

Há uma tonelada de mudanças para Bootstrap e por isso é impossível descreve-los tudo aqui, então aqui vai algumas das nossas mudanças favoritas:

- **Movido de Less para Sass.** Bootstrap agora compila mais rápido do que nunca, graças ao Libsass, e nós estamos cada vez mais junto com a enorme comunidade de desenvolvedores Sass.
- **Sistema de grid melhorado.** Nós adicionamos uma nova camada de grid para atender melhor dispositivos móveis e remodelamos completamente nossos mixins semânticos.
- **Suporte Opt-in flexbox.** O futuro é agora — mudamos a variável boolean e recompilamos seu CSS para tirar proveito de um sistema de grid baseado em flexbox e componentes.
- **Alterado wells, thumbnails, e panels para cards.** Os cards são um novo componente do Bootstrap, mas com eles, vocêse sentira super a vontatde, são parecido com wells, thumbnails, and panels, só que melhor.
- **Consolidado todo reset de nosso HTML em um novo módulo, Reboot.** Reinicie etapas em Normalize.css onde parar, dando-lhe mais opções como resets `box-sizing: border-box`, ajustes de margens, e mais, tudo isso em um único arquivo Sass.
- **Novas opções de customização do Brand.** Em vez de banir enfeites de embelezamento do estilo como gradientes, transições, sombras, e muito mais para uma folha de estilo (css) separada como na v3, nós movemo-nos todas essas opções em variáveis ​​Sass. Quer transições padrão em tudo ou desativar cantos arredondados? Basta atualizar uma variável e recompilar.
- **Sem suporte para IE8 e atualização para unidades rem e em.** Fim do suporte para IE8 significa que podemos aproveitar as melhores partes de CSS sem serem mantidas com hacks CSS ou fallbacks. Pixels foram trocados por rems e ems quando apropriado para fazer tipografia ágil e dimensionamento de componente ainda mais fácil. Se você precisar de suporte IE8, continue usando Bootstrap 3.
- **Reescrito todos nossos plugins JavaScript.** Cada plugin foi reescrito em ES6 para tirar vantagem das mais recentes melhorias de JavaScript. Eles também já vêm com suporte UMD, métodos de desmontagem genéricos, tipo de opção de verificação, e toneladas mais.
- **Melhoria de auto-posição de tooltips e popovers** graças à ajuda de uma ferramenta chamada Tether.
- **Melhoria da documentação.** Nós reescrevemos tudo em Markdown e acrescentamos alguns plugins úteis para agilizar exemplos e trechos de código para tornar o trabalho com nossos docs de maneira mais fácil. Melhoria da pesquisa também é uma outra maneira.
- **E mais novidades!** Controles personalizados de formulário, classes CSS de margin e padding, novas classes de utilitários, e muito mais coisas foram incluídos.

E isso mal começou, até agora temos 1,100 commits e 120,000 linhas de alterações na v4. Além disso, não estamos sequer prontos ainda!

Pronto para conhecer-la? Então [mergulhe de cabeça na documentação v4 alpha!](http://v4-alpha.getbootstrap.com)

## Plano de Desenvolvimento

Precisamos da sua ajuda para fazer Bootstrap 4 o melhor possível. A partir de hoje, o código fonte para v4 estarão disponíveis em no [branch `v4-dev` no GitHub](https://github.com/twbs/bootstrap/tree/v4-dev). Além disso, temos uma [v4 development and tracking pull request](https://github.com/twbs/bootstrap/pull/17021) que inclui um checklist master para verificar mudanças que fizemos e os nossos possíveis restantes afazeres. Adoraríamos a ajuda de todos vocês.

O desenvolvimento e lançamento plano geral é algo como isto:

- Algumas versões alpha enquanto as coisas ainda estão em fluindo.
- Duas versões beta após recursos e funcionalidades forem fechados para que possamos realmente testar as coisas.
- Duas versões candidates (RCs) para realmente testar as coisas mais perto de ambientes de produção.
- Em seguida, a versão final!

Para aqueles que quiserem conversar sobre a v4 com a gente, nós também temos um canal Slack v4 dedicado. Converse de negócios e trabalhos com seus companheiros de Bootstrappers. Se você ainda não tiver, [junte-se à nossa sala oficial Slack!](https://bootstrap-slack.herokuapp.com).

Se você não estiver interessado em enviar código para v4, nós adoraríamos ouvi-lo em nosso [gerenciador de tarefas](https://github.com/twbs/bootstrap/issues/) com sugestões de bugs, perguntas e comentários gerais.

## Suporte para v3

Quando nós lançamos Bootstrap 3, nós imediatamente interrompido todo suporte para v2.x, causando muita dor para todos os nossos usuários pelo mundo a fora. Isso foi um erro que não vai fazer novamente. Para o futuro próximo, nós estaremos mantendo Bootstrap 3 com correções de bugs críticos e melhorias de documentação. A documentação do v3 também continuará hospedada após lançamento da v4 final.

## Mais uma coisa...

Além de divulgarmos a primeira versão alphao do Bootstrap 4 hoje, estamos também lançando nosso projeto paralelo mais recente, [Official Bootstrap Themes](http://themes.getbootstrap.com).

[![Official Bootstrap Themes](http://bootstrapbrasil.github.io/bootstrap-blog/img/2015/bs-themes.png)](http://themes.getbootstrap.com)

<!--We've talked about building premium themes for Bootstrap since our earliest releases, but never quite found the time or ideal approach until earlier this year. We've poured hundreds of hours into these themes and consider them to be much more than traditional re-skins of Bootstrap. They've very much their own toolkits, just like Bootstrap.

To start, we’re launching with three themes built on Bootstrap 3: a [dashboard](http://themes.getbootstrap.com/products/dashboard), an [application](http://themes.getbootstrap.com/products/application), and a [marketing](http://themes.getbootstrap.com/products/marketing) site. Each theme contains everything you'd find in Bootstrap, plus stunning real world examples, brand new components and plugins, custom documentation, and simple build tools.

All themes include a [multiple-use license](http://themes.getbootstrap.com/pages/our-license) for the purchaser and free updates for bug fixes and documentation updates for the life of the themes.-->

[Mergulhe de cabeça no site Bootstrap themes](http://themes.getbootstrap.com) para ve-los.

<3,

[@mdo](https://twitter.com/mdo), [@fat](https://twitter.com/fat), & [team](https://github.com/twbs)

Tradução: [@adammacias](https://twitter.com/adammacias)
