---
title: 'Customizing Mac&#8217;s bash shell and vim'
author: kanitw
layout: post
published: false
categories:
  - Developers
  - English
tags:
  - bash
  - coding
  - geek
  - lifehacking
  - Mac OSX
---

Start by enabling .bashrc adding to /etc/profile

    *[ -r $HOME/.bashrc ] && source $HOME/.bashrc*

Then start customizing it!  Here are some good guides:



*   Adding Colors: 
*   Adding Completion: using homebrew

     brew install bash-completion

(also have to add this to .bash_profile)

    if [ -f `brew --prefix`/etc/bash_completion ]; then
     . `brew --prefix`/etc/bash_completion
    fi

If have no .bash_profile yet, one easy way is to add

    source ~/bin/.bash_profile

to /etc/profile



### Vim

*   Pathogen – for easy plugin install 
*   (discovering)

As usual, feel free to comment if you have good advice!