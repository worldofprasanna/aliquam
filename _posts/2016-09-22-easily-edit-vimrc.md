---
layout: post
title:  "Vim tricks"
date:   2016-09-22 02:21:54 +0530
tags: vim tricks vimrc
---

After I became little bit comfortable with vim, I started customizing it a lot. And many times I would open the vimrc file which is in ~/.vimrc, save my changes, quit the vim and start it again to refresh my changes. It was bit painful at times because it will take more time to get feedback and I would have made a silly mistake there and I have to repeat the whole process again.

But after sometime I find this cool trick by which we can open the vimrc file within the current buffer using `:e $MYVIMRC`, so I did remap my vim keystrokes to do this work,

`
nnoremap ev :e $MYVIMRC<CR>
`

Now I can easily open the vimrc file in the current buffer and edit it.
To reload the vimrc without quitting, I can `source $MYVIMRC` and so this line came into my vimrc,

`
nnoremap rv :w!<Esc>:source $MYVIMRC<CR>
`

Once edited and reloaded, to go back to my previously opened buffer `<C-o>`

PS :-
1. $VIMRC gives the location of your vimrc file
2. [my vimrc](https://github.com/worldofprasanna/pulligal)

