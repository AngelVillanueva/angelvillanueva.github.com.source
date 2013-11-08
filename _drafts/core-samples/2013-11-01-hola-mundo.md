---
layout: post
title: "Hola mundo"
description: ""
category: nova
tags: [pepper, intro, contaminación]
comments: true
share: true
image:
  feature: abstract-7.jpg
  background: triangular.png
---
{% include JB/setup %}

This is my first post, it seems pretty simple to get a blog running.

It's time to learn some more markdown, perhaps [here] (http://www.as.com).

![An Image]({{ site.url }}/images/hpstr-jekyll-theme-preview.jpg)

Ok, do not remember how to build a link with markdown, let's see different things:


## list yes

Here `some code` to be learned, with some remarks:
* 1
* 2

# h1
Código con coderay:

~~~ ruby
some code just by tabbing
some more require 'this/that'
User.each do |u|
very interesting and awesome
~~~

~~~ html
<div>hola</div>
~~~

{% highlight php %}
  $hola = 2;
  echo $hola;
{% endhighlight %}

~~~ ruby
module Jekyll
  class TagIndex < Page
    def initialize(site, base, dir, tag)
      @site = site
      @base = base
      @dir = dir
      @name = 'index.html'
      self.process(@name)
      self.read_yaml(File.join(base, '_layouts'), 'tag_index.html')
      self.data['tag'] = tag
      tag_title_prefix = site.config['tag_title_prefix'] || 'Tagged: '
      tag_title_suffix = site.config['tag_title_suffix'] || '&#8211;'
      self.data['title'] = "#{tag_title_prefix}#{tag}"
      self.data['description'] = "An archive of posts tagged #{tag}."
    end
  end
end
~~~

Y finalmente una blockquote o como sea:

> En un lugar de la Mancha, de cuyo nombre no quiero acordarme, no ha mucho vivía un hidalgo de los de lanza en astillero, adarga antigua, rocín flaco y galgo corredor.

Fin
