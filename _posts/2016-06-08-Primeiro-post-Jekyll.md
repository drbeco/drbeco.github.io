---
layout: post
title:  "Primeiro post com Jekyll"
date:   2016-06-08 18:17:37
categories: test jekyll
---

Formato para nomes dos posts: YYY-MM-DD-titulo-do-post.md

Codigo em `linha` com acentos graves, e tantas outras facilidades da linguagem _Markdown_.

Jekyll também oferece suporte para código fonte:

{% highlight C %}
int main(int argc, char **argv)
{
    int d;

    d=getchar();
    putchar(d);

    return EXIT_SUCCESS;
}
{% endhighlight %}

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Beco')
{% endhighlight %}

Veja [Jekyll docs][jekyll] para mais informacoes. Faça fork do repositório do Jekyll para iniciar seu site.

[jekyll]:    http://jekyllrb.com

