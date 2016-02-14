---
layout: page
title: jekyll bootstrapをgithubページにインストールしてみた
tagline: jekyll
---
自前で作ってたけど、jekyll-bootstrapがかっこよかったので入れてみた。

[Blogging with Jekyll Tutorial | Jekyll-Bootstrap](http://jekyllbootstrap.com/)

    $ git clone https://github.com/plusjade/jekyll-bootstrap.git mattn.github.com
    $ cd mattn.github.com
    $ git remote set-url origin git@github.com:mattn/mattn.github.com.git
    $ git push origin master

テーマも変えた

    $ rake theme:install git="https://github.com/jekyllbootstrap/theme-twitter.git"

記事書いて

    $ vim _post/2012-03-22-installed-jekyll-bootstrap.md
    $ git add !$ && git commit -m "add"

投稿

    $ git push origin master

簡単。ローカルで確認したいなら

    $ gem install jekyll
    $ jekyll --server --auto

この辺は前に書いたのでそっちを見てね。

[Jekyllで始める簡単ブログ](http://mattn.kaoriya.net/software/lang/ruby/20090409185248.htm)

[githubとjekyllとoctopressで作る簡単でモダンなブログ](http://mattn.kaoriya.net/software/lang/ruby/20111017205717.htm)

何も触らなくていいのが便利だし、[テーマブラウザ](http://themes.jekyllbootstrap.com/)とかカッコ良すぎる。
ちなみに、分かってる人は分かってるだろうけど、octopressはmarkdownを静的にhtmlを生成してアップロードするのに対してjekyllはmarkdownのままアップロードしてgithubに処理させてるので、jekyllプラグインはgithub上で動こうとする。つまりローカルでしか動かないという事。
