# Ink
Crisp, minimal personal website and blog theme Hugo. Forked from [knadh](https://github.com/knadh/hugo-ink).

## Features
* Google Analytics integration
* Syntax highlighting
* Twitter cards and opengraph tags support
* RSS feeds
* Custom CSS/JS
* Multilingual months support

## Installation

cd into your hugo site's root directory and:

```sh
cd themes
git clone https://github.com/knadh/hugo-ink.git
```

For more information read the [official setup guide](https://gohugo.io/overview/installing/) of Hugo.


## Content type

You can specify content type with field `type` in your content. For example static pages can be set as type `page` which are excluded from recent posts and all posts page. 

```md
---
title: "About"
date: 2019-04-19T21:37:58+05:30
type: "page"
---

This is some static page where you can write about yourself.
```

## Language Settings for the month

Due to the currently unavailable feature for multilingual dates in ``.Date`` from
Go. It is possible to create a ``month.yaml`` in the data folder of your
Hugo site root directory. There is also an example file in
``exampleSite/data/``.

```sh
cat > month.yaml << EOF
1: "Jan"
2: "Feb"
3: "Mar"
4: "Apr"
5: "May"
6: "Jun"
7: "Jul"
8: "Aug"
9: "Sep"
10: "Oct"
11: "Nov"
12: "Dec"
EOF
```

## Credits

* [Ezhil theme](https://github.com/vividvilla/ezhil) from which Ink was forked

Licensed under the MIT license.
