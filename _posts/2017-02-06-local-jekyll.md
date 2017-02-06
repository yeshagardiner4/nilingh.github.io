---
layout: post
title:  "在Mac上配置GitHub pages环境"
date:   2017-02-06 14:31:00 +0800
categories: blog dev
---

使用GitHub pages搭配jekyll搭建个人博客是一个免费且简单的方案。之后应该在本地计算机上安装和运行jekyll来模拟GitHub pages环境，这样可以让你在发布任何修改之前先在本地浏览器上预览结果，调试正确后再同步到你的github里。

jekyll官网上的安装过程比较简单，我的mac之前没有配置过Ruby环境，所以安装和运行<kbd>jekyll server</kbd>的时候走了不少弯路，最后是通过<kbd>bundle install</kbd>来自动安装各种包后成功运行。

网上安装过程的文章很多，但每个人实际情况有差别，主机环境不同，个人知识面也是一个很大的因素。我自己之前没有接触过ruby，在安装过程中才了解到brew，rvm，gem，bundler这些工具。由于ruby牵涉到环境参数，包之间的依赖等，所以简单复制别人的命令可能会把自己机器的环境弄乱。建议后来的同学先浏览一下[git官网帮助文档](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/)，事后看来还是写的很清楚的，使用bundler安装，jekyll官网是使用gem安装的。

下面是一些参考步骤：

 1. 首先要配置ruby环境，更新Mac系统环境。包括安装xcode及command line tools，[brew](http://brew.sh)，rvm，ruby，bundler。[ruby-china](https://ruby-china.org/wiki/install_ruby_guide)上这个文档非常好。
 2. 参考[git官网帮助文档](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/)来配置你的本地jekyll环境。
 
因为我的blog目录中已经有了Gemfile，所以bundle install时会按照文件中jekyll的版本来安装相应需要的包

最后运行<kbd>jekyll server</kbd>，在浏览器中访问http://127.0.0.1:4000，祝大家使用愉快。



> Written with [StackEdit](https://stackedit.io/).


