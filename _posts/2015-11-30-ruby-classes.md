---
layout: post
title:  "Ruby classes"
date:   2015-11-30 16:21:19 -0600
categories: jekyll update
---
	
Have you found yourself creating a bunch of similar variables and applying the same methods over and over again? Then you need to start creating your own class objects!

Ruby classes are used to define a new type of object with a set of callable methods.

Classes use instance and local variables. Local variables can only be used inside the method where it is defined. Instance variables all start with the @ symbol. They can be used anywhere inside the class that it is defined in.
		
An example of when you might create a class is if you need to create a new rectangle and apply different formulas to it.
		
__Example:__
{% highlight ruby %}
class Rectangle
 def initialize(width=1, height=1)
  @width = width
  @height = height
 end

 def perimeter
  return 2 * (@width + @height)
 end

 def area
  return @width * @height
 end

 def diagonal
  return Math.sqrt(@width**2 + @height**2)
 end
end
{% endhighlight %}

{% highlight ruby %}
rect = Rectangle.new(3, 7)
rect.perimeter
=> 20
rect.area
=> 21
rect.diagonal
=> 7.615773105863909
{% endhighlight %}
		
By creating a new class called Rectangle, you don't need to call the various methods and pass in the same variables (for width and height) every time because the method in the class takes care of that for you. Still, you can create methods that take in arguments. You might do that if the arguments that are being passed in don't need to be used right away. Otherwise, you'd need to initialize them right away.