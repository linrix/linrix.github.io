 About this Cool Concise Jekyll Blog Theme 🤘🤘🤘

[![GitHub stars](https://img.shields.io/github/stars/linrix/linrix.github.io.svg)](https://github.com/linrix/linrix.github.io/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/linrix/linrix.github.io.svg)](https://github.com/linrix/linrix.github.io/network)
[![GitHub issues](https://img.shields.io/github/issues/linrix/linrix.github.io.svg)](https://github.com/linrix/linrix.github.io/issues)
[![GitHub release](https://img.shields.io/github/release/linrix/linrix.github.io.svg)](https://github.com/linrix/linrix.github.io/releases)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/linrix/linrix.github.io/master/LICENSE)

## Content

* [Usage](#usage)
    * [1. Install ruby and jekyll environment](#1-install-ruby-and-jekyll-environment)
    * [2. Copy theme code](#2-copy-theme-code)
    * [3. Change parameter](#3-change-parameter)
        * [Basic info](#basic-info)
        * [Link info](#link-info)
        * [Comments info](#comments-info)
        * [Statistical analysis info](#statistical-analysis-info)
    * [4. Write post](#4-write-post)
    * [5. Local launch](#5-local-launch)
    * [6. Push to GitHub](#6-push-to-github)

## Usage

Welcome everyone to use this theme, this part shows introduction to use.

### 1. Install ruby and jekyll environment

This step and Step 5 mainly talk to you how to launch blog at local. If you don't want to launch at local, you can ignore these 2 steps. But I still strongly suggest to do this. Ensure there is nothing wrong before pushing to the github.

The Windows users can directly use [RubyInstaller](http://rubyinstaller.org/) to install ruby environment. Follow the prompts while installing.

Install jekyll commands:

```
gem install jekyll
```

For more details, you can view the jekyll official website. [https://jekyllrb.com/](https://jekyllrb.com/)

There may be something wrong at mac OS X El Capitan, you can see the solution at [https://jekyllrb.com/docs/troubleshooting/#jekyll-amp-mac-os-x-1011]( https://jekyllrb.com/docs/troubleshooting/#jekyll-amp-mac-os-x-1011).

If you are interesting in jekyll, you can see the jekyll source code at [https://github.com/jekyll/jekyll](https://github.com/jekyll/jekyll).

![jekyll logo](http://jekyllcn.com/img/logo-2x.png)

### 2. Copy theme code

You can clone, download or fork this repo.

### 3. Change parameter

Mainly change the parameters at file `_config.yml` and use your own `favicon.ico`.

#### Basic info

Shows at site header part.

```yml
# Site settings
title: HyG
brief-intro: Front-end Dev Engineer
baseurl: "" # the subpath of your site, e.g. /blog
url: "http://linrix.github.io" # the base hostname & protocol for your site
```

#### Link info

Mainly shows at the footer of the site.

```yml
# other links
twitter_username:
facebook_username:
github_username:
email:
weibo_username:
zhihu_username:
linkedIn_username:
dribbble_username:

description_footer: 本站记录我前端之旅的沿途风景！
```

#### Comments info

Get your own `short_name`:

Visit https://disqus.com/ or http://duoshuo.com/. And follow the prompts at the site.

```yml
# comments
# two ways to comment, only choose one, and use your own short name
duoshuo_shortname: #hygblog
disqus_shortname: xxxx
```

When you done, you can also see the comments info at disqus or duoshuo admin console.

#### Statistical analysis info

Get Google Analytics id or Baidu Statistics id：

Visit https://www.google.com/analytics/ or http://tongji.baidu.com/. And follow the prompts at the site.

Of course, if you don't want any statistical and analysis info, you can type nothing at id position.

```yml
# statistic analysis 统计代码
# 百度统计 id，将统计代码替换为自己的百度统计id，即
# hm.src = "//hm.baidu.com/hm.js?xxxxxxxxxxxx";
# xxxxx字符串
baidu_tongji_id: cf850xxxxxxxxxxxxxxxx
google_analytics_id: UA-7xxxxxx-4 # google 分析追踪id
```

When you done, you can see UV, PV, location etc. info at your own Google Analytics or Baidu Statistic console.

### 4. Write post

You can write posts at folder `_posts`. At the beginning of the post, you should declare layout、title、date、categories、tags、author(optional) info、mathjax(optional，click [here](https://www.mathjax.org/) for more detail about `Mathjax`).

```
---
layout: post
title:  "对这个 jekyll 博客主题的改版和重构"
date:   2016-03-12 11:40:18 +0800
categories: jekyll
tags: jekyll 端口 markdown Foxit RubyGems HTML CSS
author: Haoyang Gao
mathjax: true
---
```

These follow code is for making contents.
```
* content
{:toc}
```

You can use 4 wraps as a excerpt separator. The words before separator as excerpt show in the index page. When you enter the post page, you can read full article.

The wraps config is in the file `_config.yml`, as follows:

```yml
# excerpt
excerpt_separator: "\n\n\n\n"
```

You should use markdown syntax to write article, just like write readme in github.

You can use 3 \`\`\` to write code block.

### 5. Local launch

use command:

```
jekyll s
```

Terminal shows:

```
Configuration file: E:/GitWorkSpace/blog/_config.yml
            Source: E:/GitWorkSpace/blog
       Destination: E:/GitWorkSpace/blog/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
                    done in 6.33 seconds.
  Please add the following to your Gemfile to avoid polling for changes:
    gem 'wdm', '>= 0.1.0' if Gem.win_platform?
 Auto-regeneration: enabled for 'E:/GitWorkSpace/blog'
Configuration file: E:/GitWorkSpace/blog/_config.yml
    Server address: http://127.0.0.1:4000/
  Server running... press ctrl-c to stop.
```

Visit localhost:4000 to see your blog!!!

### 6. Push to GitHub

If there is nothing wrong, push code to your github!

## License

[MIT License](https://github.com/linrix/linrix.github.io/blob/master/LICENSE.md)
