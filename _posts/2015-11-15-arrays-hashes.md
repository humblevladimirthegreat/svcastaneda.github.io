---
layout: post
title:  "Arrays vs. Hashes"
date:   2015-11-15 16:21:19 -0600
categories: jekyll update
---
Knowing whether to use an array or hash can be challenging because they both hold data that you can access. So what's the difference?
	
-----
	
###Arrays
Arrays are basically indexed lists. When I say indexed, I mean that you can retrieve data by calling an index. You would use an array when you just need a simple collection of data.

> __Example:__ If you created this array: `list = ["a", "b", "c"]` and called the index 0 like this: `list[0]`, it would return the value `"a"`.
	
-----
	
	
###Hashes
You can think of hashes like dictionaries. They have keys and values similar to how a dictionary has unique words and definitions. You wouldn't find the word "apple" listed more than once. Instead, you would find all of the various definitions listed under one word. But unlike dictionaries, hashes are unordered (except for newer versions of Ruby). So, instead of using indexes to access the data, you need to call a hash's key, which will return its value(s). Hashes are good to use when you have to map information or group data together, but the data falls under one category.

> __Example:__ If you created this hash for students in your class that are mapped by their student ID number: `students = [23148123=>"Sammy", 12381415=>"Dexter", 82373234=>"Lucy"]` and called the key 23148123 like this: `students[23148123]`, it would return the value `"Sammy"`.