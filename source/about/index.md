---
title: About Lx
date: 2021-08-17 19:45:56
comment: true
---

# Hexo-Theme-Lx

<img src="https://d33wubrfki0l68.cloudfront.net/6657ba50e702d84afb32fe846bed54fba1a77add/827ae/logo.svg" alt="logo" width="140" height="140" align="right">

[![Github Release](https://img.shields.io/github/release/blleng/hexo-theme-lx.svg)](https://github.com/blleng/hexo-theme-lx/releases/)
[![Github License](https://img.shields.io/github/license/blleng/hexo-theme-lx.svg)](https://github.com/blleng/hexo-theme-lx/blob/master/LICENSE)

>Star me if you like.

Any problem: [issue](https://github.com/blleng/hexo-theme-lx/issues)


## Usage

### Git clone

At theme blog root dir:

```bash
$ git clone https://github.com/blleng/hexo-theme-lx themes/lx
```

### Apply

Edit `_config.yml`:

```yml
theme: lx
```

## Features

### Analytics

`lx` use Baidu and Google as analytics.

Usage:

Edit `themes/lx/_config.yml`:

```yml
google_analytics: ... ##Google analytics ID
baidu_analytics: ... ##Baidu analytics ID
```

### Local search

1. Install the `hexo-generator-searchdb`:

At the blog root dir:

```bash
$ npm install hexo-generator-searchdb -s
```

2. Edit `themes/lx/_config.yml`:

```yml
local_search:
  enable: true
```

More features in `themes/lx/_config.yml`

### Comment

`lx` use valine as comment system.
The official site: [https://valine.js.org](https://valine.js.org)

Usage:

Edit `themes/lx/_config.yml`:

```yml
comment:
  enable: true
  appid: ... #leancloud appid
  appkey: ... #leancloud appkey
  notify: false
  verify: false
  placeholder: Say something #placeholder
  avatar: identicon #the guest avatar
  guest_info: nick,mail,link #optional choice
  pageSize: 10
  language: en
```

In the page front-matter:
`comment: true`

```markdown
---
date: ...
title: ...
categories: ...
tags: ...
comment: true //use comment in this page
mathjax: ...
---
```

You should create an application in Leancloud to get `appid` and `appkey`.

### Social links

Edit the `themes/_config.yml`

```yml
social:
  enable: true
  links:
    Github:  //the name of the link
      icon: gihub //font-awesmome icon
      link: ... //link
```

### Mathjax

Support Mathematical formulas and chemical equations

Usage:

Edit`themes/lx/_config.yml`:

```yml
mathjax:
  enable: true
  cdn: //cdn.bootcss.com/mathjax/2.7.5/latest.js?config=TeX-MML-AM_SVG
```

In the page front-matter: `mathjax: true`

```markdown
---
date: ...
title: ...
categories: ...
tags: ...
comment: ...
mathjax: true //use Mathjax in this page
---
```

### Font

```yml
font:
  enable: true
  host: //fonts.googleapis.com
  codes: ##the font of codes
    enable: true
    family: Fira Code
  else:
    enable: false
    family: 
```

### Custom style

```yml
custom_css: fasle
# If true, Lx will load 'source/css/custom.styl'
```