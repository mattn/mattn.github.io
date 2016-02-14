---
layout: post
title:  Jedieでサイトを作り直した。
---
jekyll-bootstrap を使ってたのだけど新規投稿が反映されない問題があったので、一旦全部消して作り直した。

使ったのはお手製の jekyll clone、[jedie](https://github.com/mattn/jedie)

```
$ jedie new .
$ vim _posts/2016-02-15-rebuild-site-with-jedie.md
$ git add .
$ git commit -a
$ git push origin master
```

jedie 便利。 :+1:
