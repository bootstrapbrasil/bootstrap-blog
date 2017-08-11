---
layout: post
title: Bootstrap 4 Alpha 5
---

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="//www.youtube.com/embed/MxGEVIvSFeY?rel=0" width="760" height="570" allowfullscreen></iframe>
</div>

[Alpha 5 foi lançado](http://v4-alpha.getbootstrap.com) apenas um mês depois do Alpha 4 com grandes melhorias de recursos e pacotão com correções de bugs. Nós ainda temos muito trabalho pela frente, mas estamos deixando mais estável a cada lançamento. Continue lendo para ver os destaques e planos do Alpha 6.

### Novos pacotes CSS

Atualizamos nosso processo de compilação para incluir versões com todos nossos pacotes CSS. Além de adicionar o padrão de longa data compilada e pacotes minificados, que incluem arquivos CSS compilados para nosso uso do modo flexbox, sistema de grids apenas, e Reiniciar apenas pacotes. Cada pacote possui um arquivo compilado, minificado, e mapa Sass, assim como o CSS tradicional.

### Grid atualizados

Nosso grid foi atualizado e está mais flexível do que nunca. Novidades no Alpha 5 são breakpoint grid gutters específicos. Isso mesmo, agora você pode personalizar a largura de gutters em cada nível e toda camada de grid, modificando o mapa Sass.

The `.container` behaviors have changed slightly in Alpha 5. We now set the `width` of each container alongside a `max-width: 100%;` to ensure proper rendering across browsers in both our default and flexbox modes. Similarly, we fixed a bug in our flexbox grid where columns didn't properly collapse at lower breakpoints.

O comportamento do `.container` foi um pouco alterado no Alpha 5. Agora vamos definir o `width` para cada container ao lado de `max-width: 100%;` para garantir que fique o modo padrão e flexbox ambos fiquem adequado em qualquer navegador. Da mesma forma, corrigimos um bug em nosso grid flexbox onde colunas não estavam adequadas em breakpoints menores. 

Por último, nós mudamos um ponto breakpoint e dimensões do container. A camada `sm` container agora está menor do que dimensões viewport e a camada `lg` foi modificada de `940px` para `960px` para o grid de 12 colunas fiquem mais limpo.

### Revisão de Utilitários

Classes utilitárias tiveram bastante atenção em Alpha 5 e vai continuar no Alpha 6. Grandes mudanças neste lançamento são:

- Simplificado sintaxe `margin` e `padding` (e.x., `mx-auto` ao invés `m-x-auto`).

- Separado utilitários `background` e `color` para o estilo ficar mais explícito.

- Renomeado utilitário image, alterado de `.img-rounded` e `.img-circle` para `.rounded` e `.rounded-circle`, respectivamente.

- Removido o `display: block;` de `.img-fluid` pois torna-se desnecessário para criar imagens responsivas (o `inline-block` padrão funciona muito bem como está).

- Adicionado novo utilitário `vertical-align` com `.align-top`, `.align-middle`, e mais.

Veja outras questões em aberto em [Alpha 6 milestone](https://github.com/twbs/bootstrap/milestone/39). Há mais atualizações vindo ao utilitários para adicionar variações responsivas, nomenclatura mais consistente e muito mais.

### Navbar atualizado

Nós dedicamos um [enorme tempo na barra de navegação para Alpha 5](https://github.com/twbs/bootstrap/pull/19890), mas honestamente, não está finalizado. Em vez de retornar o progresso que fizemos até Alpha 6, nós incluímos algumas coisas meia-boca.

Aqui está uma olhada no que há de novo, como ele funciona, e o que pode mudar no nosso próximo lançamento.

- Primeiro, a barra de navegação tem uma **novo brand toggler** que são baseada em SVG `background-image` personalizável. Com o poder de variáveis Sass, que nos permite mudar facilmente a cor dos ícones do menu de hamburger.

- Segundo, o **estilo padrão para brand e navegação em grande parte foi ajustado**. Estão com estilos global menos personalizados dando ênfase no posicionamento e flexibilidade.

- Building on that, we **overhauled the collapse plugin integration for responsive navbars**. With the help of some utility classes and collapse classes for each grid tier, you can easily pick the breakpoint for collapsing your navbar without having to recompile your Sass. Also included is the auto restyling of dropdown menus for mobile so they no longer hide other navbar content when toggled.

- Com base nisso, nós **reformulados a integração do plugin collapse para barra de navegação responsiva**. Com a ajuda de algumas classes utilitárias e collapse para cada camada de grid, você pode facilmente escolher o breakpoint para recolher a sua barra de navegação sem ter que recompilar seu Sass. Também está incluído o auto re-estilo de menus suspensos em celular para que eles não escondem outros conteúdos navbar quando alternado.

A barra de navegação é um complicado um há tanta funcionalidade e estilo que pode ir com elas. Temos [próximo esboços de grandes pedaços para a barra de navegação](https://github.com/twbs/bootstrap/issues/20937), mas provavelmente há mais que estamos gostaríamos. Certifique-se de estar com componente atualizado antes de seu feedback.

### Chegando o Alpha 6

Estamos pensando em mais um grande lançamento alpha antes de entrar nas versões beta e mais estáveis. Ainda há mais a fazer em torno de nossos principais componentes — a barra de navegação, variantes flexbox, utilitários e accessibilty — para seguirmos em frente.

Uma vez feito isso, vamos rever toda nossa documentação e atualizar todos os nossos modelos de exemplos para os mais recentes. A partir daí vamos precisar de sua ajuda para testar essas alterações e reportar bugs. Fique atento para mais atualizações na medida que nos aproximamos para que a liberação.

Até lá, fique com Alpha 5!

---

Para mais detalhes sobre esse lançamento, dê uma olhada na [lista de issues Alpha 5](https://github.com/twbs/bootstrap/issues/20630), assim como a bem como a [a lista de melhorias já realizadas Alpha 5](https://github.com/twbs/bootstrap/milestone/36?closed=1). Lembre-se de participar da [nossa sala no no Slack @BootstrapBrasil!](http://bootstrapbrasil-slack.herokuapp.com).

**Usando o Bootstrap CDN?** Reveja as alterações e atualize seus links CDN para apontar para os arquivos mais recentes:nd update your CDN links to point to the latest files:

{% highlight html %}
<!-- Última versão CSS compilada e minificada -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.5/css/bootstrap.min.css" integrity="sha384-AysaV+vQoT3kOAXZkl02PThvDr8HYKPZhNT5h/CXfBThSRXQ6jW5DO2ekP5ViFdi" crossorigin="anonymous">

<!-- Última versão JavaScript compilada e minificada -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.5/js/bootstrap.min.js" integrity="sha384-BLiI7JTZm+JWlgKa0M0kGRpJbF2J8q+qreVrKBC47e3K6BW78kGLrCkeRX6I9RoK" crossorigin="anonymous"></script>
{% endhighlight %}

<3,<br>
[@mdo](https://twitter.com/mdo) & [team](https://github.com/twbs)

Tradução: [@adammacias](https://twitter.com/adammacias)
