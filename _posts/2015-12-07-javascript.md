---
layout: post
title:  "Looping in Ruby vs. Looping in JavaScript"
date:   2015-12-07 16:21:19 -0600
categories: jekyll update
---
	
Recently, I began learning JavaScript. While Ruby and JavaScript are pretty similar, there's one major difference that I believe is one of the most important things: how to iterate through arrays.

Ruby makes things easy by providing a builtin method called `each`. This method allows you to loop through all of the elements/values inside an array.

JavaScript is not as friendly. It doesn't allow you to access the individual element of an array. Instead, you have to iterate through the indexes.

You're probably wondering what I mean by "iterating through indexes." It's easier to see an example of Ruby looping vs. JavaScript looping.

__Ruby:__
{% highlight ruby %}
list = ['a', 'b', 'c', 'd']
list.each do |letter|
 p letter
end

=> 'a'
=> 'b'
=> 'c'
=> 'd'
{% endhighlight %}

__JavaScript:__
{% highlight ruby %}
var list = ['a', 'b', 'c', 'd'];
for (var i = 0; i > list.length; i++) {
  console.log(list[i]);
};

 > a
 > b
 > c
 > d
{% endhighlight %}
		
As you can see in the JavaScript example, I had to pass in an integer as the index in order to get each value in the list. Ruby takes care of that, which allowed me to simply print letter.