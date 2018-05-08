---
layout: post
title:  "Python Strings"
date:   2016-08-13 02:21:54 +0530
categories: python basics string
---
I started reading about python recently and could found that manipulating strings in python is lot more easier than java. Though i didn t like few ways of manipulating like string concatenation, but found it to be quite useful.

**Triple Quot**

Strings can be created with single quot or double quot and one by default escapes other. But there is one more way to create strings and it is with triple double quot or triple single quoti. It can be as

```
str="""This is a string
along with the 'new line'
and \t tabs as well"""

print(str)

#This is a string
#along with the 'new line'
#and \t tabs as well

```

Its very easy to create strings with new line and with single quots without escaping it. Similarly if the string contains double quots can be easily created with triple single quots without escaping. Quite handy.

**Raw String**

This is one interesting gotcha. If we need the string to be as it is, then can be prefixed with r and the string will not be interpolated for \ and other stuffs.

```
str=r'temp\t\n'
print(str)
# temp\t\n
```

**String concatenation**

Strings can be easily concatenated like other languages using +=, +. But there is one more way to concatenate,

```
str='Python''String'
print(str)
# PythonString
```

Though I don t like this in particular coz it doesn t look like a proper way to concatenate. Atleast + should be there to be explicit.

**Escape character**

Strings can easily continue over the next line with \ at the last. Yes it is available in other languages as well but it is a good feature.
```
str = "this is line one\
 and another line\
 third"

print(str)
#this is line one and another line third
```

But there will be no line breaks or \n in the string.


