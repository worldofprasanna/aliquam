---
layout: post
title:  "Proxy pattern in python"
date:   2016-08-22 02:21:54 +0530
tags: python proxy-pattern design-pattern
---

I was learning python by implementing the design patterns and this is the [github link](https://github.com/worldofprasanna/DesignProblems), also was parallely doing [Python Koans](https://github.com/gregmalcolm/python_koans) which is a very good resource to learn python.

In one of the exercises, implemented the proxy pattern using python ``dunder methods``. It was bit challenging but a good learning experience.

{% gist 24f8ee725155165c8566650a406c789d proxy-pattern.py %}

Things to note are the 2 dunder methods ``(__setattr__ and __getattr__)``, which gets called when no method matches in the Proxy class. In this dunder method, we are dynamically calling the actual method in the servicing class.

Because we are overriding the ``__getattr__ & __setattr__``, we couldn t directly assign values in the init coz it will call the dunder method and it will set in the servicing class instead of the Proxy class.

But we can use object s ``__setattr__`` method and set the properties in self. By this way we won t invoke setattr of the Proxy class.
