# Pithy

A new theme for [Hexo](https://hexo.io/).

[主题诞生记（中文的）](http://blog.shenqh.com/2016/02/24/my-hexo-theme-pithy/)

## Design idea
What i want:

* fast
* tidy
* pithy
* responsive

### how

* No script(except disqus comment and google analytics lisk), just use effective css. So first paint vaaaaaary fast.
* Responsive design, as it's no script, so no navbar-collapse here.
  * Due way: use navbar overflow hidden. Hidden the overflow element.
  * Instead: add a link page to show all other link and ensure it won't be hidden.
  * add page: hexo new page 'link'
* One css file.
* No i18n problem, nothing another if not manual add. It's very pithy.
*


## Preview
[Preview](http://blog.shenqh.com), and this is my blog.

Desktop:
![desktop](http://blog.shenqh.com/picture/hexo-theme-pithy/desktop.jpg)
Desktop archive page:
![desktop](http://blog.shenqh.com/picture/hexo-theme-pithy/desktop-archive.jpg)
pad:
![pad](http://blog.shenqh.com/picture/hexo-theme-pithy/pad.jpg)
phone:
![phone](http://blog.shenqh.com/picture/hexo-theme-pithy/phone.jpg)


## Installation

### Install

``` bash
$ git clone https://github.com/shenqihui/hexo-theme-pithy.git themes/pithy
```

### Enable

Modify `theme` setting in `_config.yml` to `pithy`.

add plugin for hexo:
```
npm install hexo-renderer-jade --save
npm install hexo-renderer-less --save
```

### Update

``` bash
cd themes/pithy
git pull
```

### Hexo Configuration
here is what must define in hexo's config file `_config.yml`, not the theme's config.

* date_format
* title

## Theme Configuration

``` yml
# Header
menu:
  Home: /
  Archives: /archives
  Link: /link
  About: /about
  Rss: /atom.xml

rss: /atom.xml

# less config
less:
  paths:
    - css/app.less

# Miscellaneous
google_analytics:
baidu_analytics:
favicon: /favicon.ico
twitter:
google_plus:
fb_admins:
fb_app_id:

# footer word
footer_word: word show at footer.

# page excerpt
excerpt:
  enable: true
  length: 100

# tagcloud, in developing, just use default.
tagcloud:
  start_color: '#777777'
  end_color: '#111111'
```