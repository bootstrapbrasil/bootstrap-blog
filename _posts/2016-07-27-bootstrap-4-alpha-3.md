---
layout: post
title: Bootstrap 4 Alpha 3
---

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="//www.youtube.com/embed/xFrGuyw1V8s?rel=0" width="760" height="570" allowfullscreen></iframe>
</div>

Alpha 3 pousou! Nós temos o sistema de grid reformulado, controles de formulários atualizados, um novo acervo de fonte, toneladas de correções de bugs, e muito mais. Tem sido vários meses desde a nossa última atualização, mas o tamanho dessa atualização deve ajudar-nos de volta aos trilhos.

Os trabalhos sobre Alpha 3 iniciou bastante amplo, abordando correções de bugs e atualizações de docs de todas as formas e tamanhos, mas terminou com um foco estreito em nossos controles de formulário e sistema de grid. Se você seguiu o desenvolvimento no nosso branch `v4-dev`, você já deve estar familiarizado com algumas destas mudanças maiores.

[Ir para o site da docs do alpha atualizada](http://v4-alpha.getbootstrap.com), or continue lendo para mais destaques.

## Sistema de grid

O sistema de grid foi revisado com três grandes pull requests—[#19099](https://github.com/twbs/bootstrap/pull/19099), [#20349](https://github.com/twbs/bootstrap/pull/20349), e [#20361](https://github.com/twbs/bootstrap/pull/20361). Esses grandes PRs foram voltada para as seguintes mudanças:

- Nossas classes de grid (containers e columns) estão agora atrás de uma variável Sass, que significa **classes de grid pode ser facilmente desativada através do Sass**. Atualize a variável booleana `$enable-grid-classes` e recompile para então removê-los.

- **As classes modificadoras do Grid estão mais simples** e não requerem mais o prefixo `col-`. Por exemplo, ao invés de `.col-offset-*-*`, `.col-push-*-*`, e `.col-pull-*-*`, nós temos `.offset-*-*`, `.push-*-*`, e `.pull-*-*`.

- **Mixins foram alterados**, e depois mudou de novo, um esforço para manter as classes geradas simples e cooperativa entre os modos standard e flexbox. Nossos dois mixins primário de coluna agora são `make-col-ready`, que abriga o `position`, `padding-*`s, e `min-height` (para evitar o colapso de colunas vazias), e `make-col` e configurando o `float` e `width`.

- ** Adicionado uma seção de personalização de grid no docs** para exemplicar como alterar o número de colunas, pontos de interrupção da linha de grid, larguras de container, e muito mais.

Estas alterações estão disponíveis em nosso standard grid, assim como a nosso flexbox grid. Mais sobre isso abaixo.

## Flexbox

<img alt="Flexbox auto-layout" src="{{ site.baseurl }}/img/2016/07/flex-cols.png" style="padding: 4px; border: 1px solid #eee;">

O modo flexbox foi atualizado no Alpha 3, a partir do sistema de grid (ele usa a mesma variável e os mixins Sass atualizados) e movendo-se através dos nossos serviços públicos e componentes.

-. **Novo docs flexbox grid** Além do docs standard grid, agora temos uma página no docs dedicado para nosso flexbox grid como ele se comporta de forma ligeiramente diferente do que o standard grid. Esta nova página inclui detalhes e maneira sobre como esse grid funciona, assim como exemplos de código adicionais.

- **Largura da coluna automática** com novas classes `.col-{breakpoint}`. Por exemplo, para o breakpoint de três colunas de largura iguais `xs`, você criar três colunas com cada uma com apenas `.col-xs`.

- **Novas classes utilitárias de alinhamento flexbox** para a distribuição dos itens verticalmente e horizontalmente. Funciona com nosso flexbox grid, bem como apenas sobre qualquer outro componente personalizado.

## Formulários

<img alt="Form validation states" src="{{ site.baseurl }}/img/2016/07/forms.png" style="padding: 4px; border: 1px solid #eee;">

Formulários tiveram várias alterações durante o início do desenvolvimento do Alpha 3. Documentação, nomes de classe, opções de layout e estilos de validação têm sido drasticamente melhorada.

- **Novas classes para checkboxes, radios, tamanhos de input e legends.** Embora não seja 100% finais, todos os nossos controles de formulário estão nomeados de forma mais clara e consistente em toda a sua CSS.

- **Substituido as imagens de fundo PNG base64 com [inline SVGs](https://github.com/twbs/bootstrap/pull/17222)** para seus controles de formulários personalizados e estados de validação. Dimensione esses controles de formulário para o conteúdo do seu coração!

- Falando de estados de validação, temos **a nova identidade de validação dos formulários com opções de texto de ajuda**. Estados de validação podem agora ser aplicada em uma base (com `.form-control-{state}`) e opcionalmente com feedback de validação pode ser mostrado com `.form-control-feedback`. Agora o texto do formulário de ajuda independente pode ser controlada com a nova classe `.form-text`.

{% highlight html %}
<div class="form-group has-success">
  <label class="col-form-label" for="inputSuccess1">
    Input with success
  </label>
  <input type="text" class="form-control form-control-success" id="inputSuccess1">
  <div class="form-control-feedback">
    Success! You've done it.
  </div>
  <small class="form-text text-muted">
    Example help text that remains unchanged.
  </small>
</div>
{% endhighlight %}

- Corrigido alguns bugs relacionados com formulário, como o preenchimento da label horizontal [#17498](https://github.com/twbs/bootstrap/issues/17498), uso indevido de `<fieldset>`s para formar grupos, classes de tamanho não aplicados nos `<select>`s, e muito mais.

- **Documentação para formulários foi revisada.** Temos exemplos mais simples de nossos controles de formulários disponíveis, orientações mais claras sobre os estados de validação (e quando usar cada um), e muito mais.

## Sistema de fonts

Nós substituímos as velha familia de font Helvetica/Arial [por fontes do sistema](https://github.com/twbs/bootstrap/pull/19098), utilizadas mais hoje em dia, mais legível, e fonts mais poderosas que empresas como a Apple, Google e Microsoft têm projetado especificamente para dispositivos de hoje.

Originalmente isso foi planejado afetar os usuários do Linux, mas esse tipo de suporte é um pouco inconsistente. Por essa razão, não há nenhuma mudança de fonts destinado a pessoas que usam Linux.

## E muito mais ...

Haviam cerca de 1.200 commits no Alpha 3 e este post mal pouco fala de todas as mudanças. Temos dezenas de outros bugs corrigidos e outras coisas melhoradas, como tambem nossa documentação.

- [Melhorado o formulário e tamanhos de botões](https://github.com/twbs/bootstrap/pull/19121)
- [Limpeza das váriavéis do componente de navegação/menu](https://github.com/twbs/bootstrap/pull/18783)
- [Renomeados contorno de botões](https://github.com/twbs/bootstrap/pull/18772) e [contorno de cards](https://github.com/twbs/bootstrap/pull/18774)
- Novas classes, variáveis e várias outras coisas!

Para mais detalhes sobre as mudanças desse lançamento, visite nossa [lista de issue Alpha 3](https://github.com/twbs/bootstrap/issues/18480), como tambem as [milestone já fechadas do  Alpha 3](https://github.com/twbs/bootstrap/milestone/35?closed=1).

**Ancioso para experimentar? Então [visite nossa docs v4 alpha!](http://v4-alpha.getbootstrap.com)**

Certifique-se de se [juntar a nossa sala no Slack! (Em Português)](http://bootstrapbrasil-slack.herokuapp.com/) ou tambem na [sala no Slack! (Em Inglês)](https://bootstrap-slack.herokuapp.com) e mergulhe em nossas novidades e relatórios de bugs, perguntas e receba nosso feedback geral sempre que possível.

## Qual é a próxima etapa?

Mais exploração, mais correções de bugs, mais atualizações de docs, e, o melhor de tudo, mais alphas. O trabalho diário nos mantém super ocupado estes dias, mas vamos fazer o nosso melhor para manter o ritmo. Fique ligado!

<3,<br>
[@mdo](https://twitter.com/mdo) & [team](https://github.com/twbs)

Tradução: [@adammacias](https://twitter.com/adammacias)
