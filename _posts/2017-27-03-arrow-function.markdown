---
layout: post
title:  "Arrow functions, ES6!"
date:   2017-03-27 09:18:00
categories: Javascript ES6 EcmaScript
---

As arrow functions a princípio podem parecer confusas (experiência própria (◕︵◕)), mas depois de um tempo, é possível entender sua sintaxe mais curta e a mágica do escopo do this.


<strong> Código sem arrow functions </strong>

{% highlight javascript %}

var oldWay = function(name, nickname) {
  return 'My name is ' + nickname + ', ' + name;
};

console.log( oldWay('James Bond', 'Bond') );
// My name is Bond, James Bond

{% endhighlight %}

<strong> Código com arrow functions </strong>

{% highlight javascript %}

let newWay = (name, nickname) => {
  return 'My name is ' + nickname + ', ' + name;
};

console.log( newWay('James Bond', 'Bond') );
// My name is Bond, James Bond

{% endhighlight %}


<strong> De uma maneira mais curta </strong>

{% highlight javascript %}
let newWay2 = (name, nickname) => 'My name is ' + nickname + ', ' + name;

console.log( newWay2('James Bond', 'Bond') );
// My name is Bond, James Bond

{% endhighlight %}

Com somente um parâmetro, não é nem necessário o uso dos parenteses

<strong> Código sem arrow functions </strong>

{% highlight javascript %}

var newWay = function(name) {
  return 'My name is ' + name;
};

console.log( newWay('James Bond') );
// My name is James Bond

{% endhighlight %}

<strong> Código com arrow functions </strong>

{% highlight javascript %}

let newWay = name => {
  return 'My name is ' + name;
};

console.log( newWay('James Bond') );
// My name is James Bond

{% endhighlight %}

