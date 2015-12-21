---
layout: post
title:  "Classes vs. IDs"
date:   2015-11-10 16:21:19 -0600
categories: jekyll update
---
Knowing whether to use a class or ID can be confusing when you're first starting to learn HTML. Even experienced people sometimes struggle with this decision! They're basically used to give specified names to certain HTML elements. But what *is* the difference?
		
-----
		
###Classes
These are used for when you have multiple HTML elements that are similar to each other. Classes can be used more than once in an HTML page and elements can have more than one class. For instance, you may have multiple divs (like a bunch of blog post previews) that all require the same (or most of the same) styling. You can refer to classes in CSS by putting a dot in front of its name.

> __Example:__ If the class name is `content`, then you would refer to it as `.content`
		
-----
		
###IDs
These are used for unique elements. You can use an ID only once in an HTML page and each element can have up to one ID. If you do not follow these conventions, your HTML will fail validation. An example of when you might use an ID is if you have a div where users can login. You can refer to IDs in CSS by putting an octothorp in front of its name.

> __Example:__ If the ID name is `loginDiv`, then you would refer to it as `#loginDiv`
