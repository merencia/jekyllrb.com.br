---
layout: docs
title: Uso Básico
prev_section: installation
next_section: structure
permalink: /docs/usage/
---

A gem Jekyll disponibiliza o executável `jekyll` em seu Terminal. 
Você pode usar este comando de várias maneiras:

{% highlight bash %}
$ jekyll build
# => A pasta corrente será gerada em ./_site

$ jekyll build --destination <destino>
# => A pasta corrente será gerada em <destino>

$ jekyll build --source <origem> --destination <destino>
# => A pasta <origem> será gerada em <destino>

$ jekyll build --watch
# => A pasta corrente será gerada em ./_site,
#    observando as alterações e regerando automaticamente.
{% endhighlight %}

Jekyll também vem com um servidor de desenvolvimento embutido que permitirá 
que você visualize o site gerado em seu navegador localmente.

{% highlight bash %}
$ jekyll serve
# => Um servidor de desenvolvimento será executado em http://localhost:4000/

$ jekyll serve --detach
# => O mesmo que `jekyll serve` mas separado de seu terminal.
#    Se você precisar parar o servidor, poderá executar `kill -9 1234` onde "1234" é o PID.
#    Se você não consegue encontrar o PID, então execute, `ps aux | grep jekyll` e finalize a instância. [Leia mais](http://unixhelp.ed.ac.uk/shell/jobz5.html).

$ jekyll serve --watch
# => O mesmo que `jekyll serve`, mas observando os arquivos e regerando automaticamente.
{% endhighlight %}

Estas são apenas algumas das [opções configuração](../configuration/).
Muitas opções podem ser especificadas através de flags por linha de comando,
ou alternativamente (e mais comumente) podem ser especificadas no arquivo `_config.yml`
na raiz do diretório de origem. Quando executar o Jekyll usará automaticamente as opções deste arquivo. Por exemplo, se você adicionar as seguintes linhas em seu arquivo `_config.yml`:

{% highlight yaml %}
source:      _source
destination: _deploy
{% endhighlight %}

Então o seguinte comando será equivalente:

{% highlight bash %}
$ jekyll build
$ jekyll build --source _source --destination _deploy
{% endhighlight %}

Para saber mais sobre as possíveis opçoes de configuração veja a página de
[configuração](../configuration/).
