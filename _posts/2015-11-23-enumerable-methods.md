---
layout: post
title:  "Ruby's map method"
date:   2015-11-23 16:21:19 -0600
categories: jekyll update
---
		
To a beginner, the map method may seem intimidating. But fear not, young padawan! The map method can be a very good friend once you understand how it works!

Basically, map iterates through a range of numbers, array, or hash and implements a block of code to each item. Map without the bang operator (!) are non-destructive, while map with the bang (!) is destructive. To be non-destructive means to return an altered clone of the original data. To be destructive is to alter the original given data.
		
__Structure on how to use map:__ {% highlight ruby %}(data).map { |obj| block } {% endhighlight %}


__Example (non-destructive version):__
{% highlight ruby %}
2.1.5 :001 > names = ['Saundra', 'Jonathan', 'Megan', 'Eddie', 'Alex']
 => ["Saundra", "Jonathan", "Megan", "Eddie", "Alex"]
2.1.5 :002 > names.map {|name| p "Hello " + name}
"Hello Saundra"
"Hello Jonathan"
"Hello Megan"
"Hello Eddie"
"Hello Alex"
 => ["Hello Saundra", "Hello Jonathan", "Hello Megan", "Hello Eddie", "Hello Alex"]
2.1.5 :003 > names
 => ["Saundra", "Jonathan", "Megan", "Eddie", "Alex"]
2.1.5 :004 >
{% endhighlight %}
		
As you can see, using the map method did not alter the original array.