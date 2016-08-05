---
layout: post
title:  "Understanding yield and blocks in Ruby"
date:   2016-08-05 11:35:38
categories: books
---
## Why do we need yield and blocks in Ruby?

Yield and blocks make your code DRYer. The same method can be used to work
in different ways. The yield key word lets you replace with a block of code
you choose making it more versatile to use. Instead of having 4 methods you will
probably dealing with 1 method and 4 blocks. In case you want to extend the
functionality you can create another block and use the same method.

The best explanation I have seen for this is [in this article](http://mixandgo.com/blog/mastering-ruby-blocks-in-less-than-5-minutes)
