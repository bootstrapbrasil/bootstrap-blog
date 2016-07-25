---
layout: post
title: Lançado Bootstrap 3.3.7
version: 3.3.7
---

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/Kr0tTbTbmVA?rel=0" width="760" height="570" allowfullscreen></iframe>
</div>

Bootstrap 3.3.7 está vivo! Nós tivemos mais de 220 commits, 80 issues resolvidas e pull requests de quase 30 contribuidores desde o último lançamento. Woohoo!

Alguns destaques são:

- Adicionado suporte para jQuery 3.
- Adicionado código inline source em arquivos dentro sourcemap eliminando os erros `4xx` no CDN.
- Atualizado vários devDependencies e gems.
- Removido vendor prefixes sem suporte para `@viewport`.

Para mais detalhes, [leia o release changelog](https://github.com/twbs/bootstrap/releases/tag/v3.3.7) e o [v3.3.7 milestone](https://github.com/twbs/bootstrap/issues?q=milestone%3Av3.3.7+is%3Aclosed).

## Download Bootstrap

Download do último código-fonte lançado, assets compilados, e documentação em um arquivo ZIP direto do GitHub:

<a class="btn-link" href="https://github.com/twbs/bootstrap/archive/v3.3.7.zip">Download Bootstrap 3.3.7</a>

Visite o [repositório do projeto](https://github.com/twbs/bootstrap) ou [respositório Sass](https://github.com/twbs/bootstrap-sass) para mais opções. Lembre-se, [estamos disponível via npm](https://www.npmjs.org/package/bootstrap) tambem.

## Bootstrap CDN

Depois de analisar o changelog, atualize seus links CDN para apontar para os arquivos v3.3.6:

{% highlight html %}
<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

<!-- Optional theme -->
<link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">

<!-- Latest compiled and minified JavaScript -->
<script src="//maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
{% endhighlight %}

<3,

[@cvrebert](https://twitter.com/cvrebert) & [team](http://getbootstrap.com/about/#team)

Tradução: [@adammacias](https://twitter.com/adammacias)
