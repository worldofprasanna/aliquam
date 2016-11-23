---
layout: post
title:  "Vim in zsh shell"
date:   2016-08-22 02:21:54 +0530
tags: vi vim zsh customization
---

I started using Vim some 6 months ago and felt this has to be my way of editing the source files. I felt I was more productive and editing source code became more fun this time.

Recently one of my friend suggested to use vi mode in the zsh shell. I was not aware that am using the default emacs mode and felt that CTRL + A, CTRL + E little awkward at times, but was living with it. So as per his suggestion, I added the line

`set -o vi`

in my `.zshrc` file and eventhough it was good to have all the key bindings now, I felt little bit difficult mainly because of 2 reasons,

**No Reverse Search**

Somehow I became a fan of CTRL + r and was getting the commands from history. I googled for this feature and found this [awesome suggestion](http://unix.stackexchange.com/questions/44115/how-do-i-perform-a-reverse-history-search-in-zshs-vi-mode/273672#273672?newreg=26e81cf912814bd590410b408c30851a).

Good part is below the accepted answer which was true vim way of doing things. We can search using `/` and `?` and use `n` and `N` to go back in the history. Very useful answer.

**Indicator of the mode**

There was no visual indicator of whether am in the normal mode or in the insert mode. Again did another googling and found this [next awesome suggestion](http://coryklein.com/vi/2015/09/17/a-working-vi-mode-indicator-in-zsh.html). It will add `NORMAL` text to the prompt when in normal mode and it was blissful.

Now happily ever after will use the `set -o vi`

**Edit long commands easily**

Though its not feature specific to vim, want to mention it here. If you are editing very big command and you want to open the command in the editor, make some changes (Though I didn t use it, coz its vim in command line, so it can be edited in commandline using vim bindings), it can be done so by pressing 'v' for vim mode. To enable this,

```
  autoload edit-command-line
  zle -N edit-command-line
  bindkey -M vicmd v edit-command-line
```
[Thanks to yoo1I](https://news.ycombinator.com/item?id=12928568) This trick worked for me.
