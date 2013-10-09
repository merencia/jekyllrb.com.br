---
layout: docs
title: Guia de início rápido
prev_section: home
next_section: installation
permalink: /docs/quickstart/
---

Para quem é impaciente, aqui está um boilerplate Jekyll rodando.

{% highlight bash %}
~ $ gem install jekyll
~ $ jekyll new myblog
~ $ cd myblog
~/myblog $ jekyll serve
# => Now browse to http://localhost:4000
{% endhighlight %}

Isso não é nada, no entanto. A verdadeira mágica acontece quando você começa a criar
posts, usando o front-matter para controlar os templates e layouts, e aproveitando
as incriveis opções de configurações disponíveis que tornar o Jekyll incrivel.

<div class="note info">
  <h5>Redcarpet é a engine Markdown padrão para novos sites</h5>
  <p>No Jekyll versão 1.1, nós trocamos a engine markdown padrão para gerar
     sites com <code>jekyll new</code> to Redcarpet</p>
</div>

Se você tem problemas quando está executando, garanta que tenha
todas as [dependências instaladas][Installation].

[Installation]: /docs/installation/
