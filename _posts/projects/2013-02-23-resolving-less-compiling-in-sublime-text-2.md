---
layout: post
title: "Resolving Less compiling in Sublime Text 2"
description: ""
category: "Hack"
tags: [solving]

---
{% include JB/setup %}

Writing CSS can be a big mess.  The dynamic stylesheet language like [Less](http://lesscss.org) is definitely a better solution.

However, Less.app is Mac is problematic (it often just stops working.)

As Sublime Text 2 is my Swiss Army Knife, another solution to deal with this is using the [Less-build-sublime](https://github.com/berfarah/LESS-build-sublime) plugin.

However, the instruction on the web does not work properly for me.

I resolved this issue by installing node.js from brew and install less from Node.js's npm

    brew install node
    sudo npm install --global less

From the log:

    npm http GET https://registry.npmjs.org/less
    npm http 200 https://registry.npmjs.org/less
    npm http GET https://registry.npmjs.org/less/-/less-1.3.3.tgz
    npm http 200 https://registry.npmjs.org/less/-/less-1.3.3.tgz
    npm http GET https://registry.npmjs.org/ycssmin
    npm http 200 https://registry.npmjs.org/ycssmin
    npm http GET https://registry.npmjs.org/ycssmin/-/ycssmin-1.0.1.tgz
    npm http 200 https://registry.npmjs.org/ycssmin/-/ycssmin-1.0.1.tgz
    /usr/local/share/npm/bin/lessc -> /usr/local/share/npm/lib/node_modules/less/bin/lessc
    less@1.3.3 /usr/local/share/npm/lib/node_modules/less
    └── ycssmin@1.0.1

I then add the path to lessc to the path config in *LESS-normal.sublime-build-choice* file in the Less-build-sublime package folder (/Users/*username*/Library/Application Support/Sublime Text 2/Packages/LESS-build)

    "path": :/usr/local/bin:$PATH"

to

    "path": "/usr/local/share/npm/bin/:/usr/local/bin:$PATH"

And then cmd+b in sublime text would just work!

