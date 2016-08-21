---
layout: post
title:  "Introduction to traits in Rust"
date:   2016-08-15 12:00:00
categories: jekyll update
---

It's been more than 6 months since I wrote my first Rust code, but it's been only a week since I started taking Rust seriously. The reason is pretty simple, Rust is awesome! I've also coming across some really exciting hacks in Rust, and so I really wanted to experience the pleasure of knowing Rust. The best resource apart from the [official docs][docs] is [Rust by example][rust-by-example]. 

so here's some rust Trait code:

{% highlight rust %}
trait Transform<Input> {
    type Output;

    fn transform(self, input: Input) -> Self::Output;
    //why the capital Self?
}
{% endhighlight %}

[docs]:https://doc.rust-lang.org/book/
[rust-by-example]:http://rustbyexample.com
