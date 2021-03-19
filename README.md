# [TeXt Theme](https://github.com/kitian616/jekyll-TeXt-theme)

[![license](https://img.shields.io/github/license/kitian616/jekyll-TeXt-theme.svg)](https://github.com/kitian616/jekyll-TeXt-theme/blob/master/LICENSE)
[![Gem Version](https://img.shields.io/gem/v/jekyll-text-theme.svg)](https://github.com/kitian616/jekyll-TeXt-theme/releases)
[![Travis](https://img.shields.io/travis/kitian616/jekyll-TeXt-theme.svg)](https://travis-ci.org/kitian616/jekyll-TeXt-theme)
[![Tip Me via PayPal](https://img.shields.io/badge/PayPal-tip%20me-1462ab.svg?logo=paypal)](https://www.paypal.me/kitian616)
[![Tip Me via Bitcoin](https://img.shields.io/badge/Bitcoin-tip%20me-f7931a.svg?logo=bitcoin)](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/docs/assets/images/3Fkufxcw2xd8HnaRJBNK4ccdtkUDyyNu4V.jpg)

![TeXt Theme](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/TeXt-home.jpg)

![TeXt Theme Details](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/TeXt-layouts.png)

TeXt is a super customizable Jekyll theme for personal site, team site, blog, project, documentation, etc. Similar to iOS 11 style, it has large and prominent titles, round buttons and cards.

**[Change Log](https://github.com/kitian616/jekyll-TeXt-theme/blob/master/CHANGELOG.md)** | **[中文](https://github.com/kitian616/jekyll-TeXt-theme/blob/master/README-zh.md)**

## Features

- Responsive
- Semantic HTML
- Skins
- Highlight Theme
- Internationalization
- Search
- Table of contents
- Authors
- Additional styles (alert, tag, image, icon, button, grid, etc)
- Extensions (audios, videos, slides, demos)
- Markdown enhancements ([MathJax](https://www.mathjax.org/), [mermaid](https://mermaidjs.github.io/), [chartjs](http://www.chartjs.org/))
- Sharing ([AddToAny](https://www.addtoany.com/), [AddThis](https://www.addthis.com/))
- Comments ([Disqus](https://disqus.com/), [Gitalk](https://gitalk.github.io/), [Valine](https://valine.js.org/en/))
- Pageview ([LeanCloud](https://leancloud.cn/))
- Analytics ([Google Analytics](https://analytics.google.com/analytics/web/))
- RSS ([jekyll-feed](https://github.com/jekyll/jekyll-feed))

## Skins

TeXt has 6 built-in skins, you can also set up your own skin.

| `default` | `dark` | `forest` |
| --- |  --- | --- |
| ![Default](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/skins_default.jpg) | ![Dark](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/skins_dark.jpg) | ![Forest](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/skins_forest.jpg) |

| `ocean` | `chocolate` | `orange` |
| --- |  --- | --- |
| ![Ocean](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/skins_ocean.jpg) | ![Chocolate](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/skins_chocolate.jpg) | ![Orange](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/skins_orange.jpg) |

### Highlight Theme

TeXt use [Tomorrow](https://github.com/chriskempson/tomorrow-theme) as the highlight theme.

| `tomorrow` | `tomorrow-night` | `tomorrow-night-eighties` | `tomorrow-night-blue` | `tomorrow-night-bright` |
| --- |  --- | --- | --- |  --- |
| ![Tomorrow](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/highlight_tomorrow.png) | ![Tomorrow Night](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/highlight_tomorrow-night.png) | ![Tomorrow Night Eighties](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/highlight_tomorrow-night-eighties.png) | ![Tomorrow Night Blue](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/highlight_tomorrow-night-blue.png) | ![Tomorrow Night Bright](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/highlight_tomorrow-night-bright.png) |

## Documentation

### Start

- [Quick Start](https://tianqi.name/jekyll-TeXt-theme/docs/en/quick-start)

- Quick For Dev

  Install docker first please

  step1: Install ( only need once in all development)

  Delete the Gemfile.lock first， or install error

  // In Windows Command Line (cmd), you can mount the current directory like so:

  ```bat
  docker run --rm -v %cd%:/usr/src/app -w /usr/src/app ruby:2.6 bundle install
  ```

  //In PowerShell, you use ${PWD}, which gives you the current directory:

  ```powershell
  docker run --rm -v ${PWD}:/usr/src/app -w /usr/src/app ruby:2.6 bundle install
  ```

  // linux

  ```shell
  docker run --rm -v "$PWD":/usr/src/app -w /usr/src/app ruby:2.6 bundle install
  ```

  step2: Build

  ```
  docker-compose -f ./docker/docker-compose.build-image.yml build
  ```

  step3:  Run

  ```shell
  docker-compose -f ./docker/docker-compose.default.yml up 
  ```

  then open the link to test, http://localhost:4000/

  

  Q:

  ```shell
  /usr/local/lib/ruby/2.7.0/rubygems.rb:277:in `find_spec_for_exe': Could not find 'bundler' (1.17.2) required by your /usr/src/app/Gemfile.lock. (Gem::GemNotFoundException)
  To update to the latest version installed on your system, run `bundle update --bundler`.
  To install the missing version, run `gem install bundler:1.17.2`
          from /usr/local/lib/ruby/2.7.0/rubygems.rb:296:in `activate_bin_path'
          from /usr/local/bin/bundle:23:in `<main>'
  ```

  https://stackoverflow.com/questions/54087856/bundler-cant-find-gem-bundler-0-a-with-executable-bundle-gemgemnotfoun

  A:
  How to fixed
  Modify the file Gemfile.lock

  ```
  BUNDLED WITH
     2.0.1
  ```

  

- [Update from 1.x to 2.x](https://tianqi.name/jekyll-TeXt-theme/docs/en/update-from-1-to-2)

### Customization

- [Configuration](https://tianqi.name/jekyll-TeXt-theme/docs/en/configuration)
- [Navigation](https://tianqi.name/jekyll-TeXt-theme/docs/en/navigation)
- [Layouts](https://tianqi.name/jekyll-TeXt-theme/docs/en/layouts)
- [Logo and Favicon](https://tianqi.name/jekyll-TeXt-theme/docs/en/logo-and-favicon)
- [Authors](https://tianqi.name/jekyll-TeXt-theme/docs/en/authors)
- [Internationalization](https://tianqi.name/jekyll-TeXt-theme/docs/en/i18n)

### Content

- [Writing Posts](https://tianqi.name/jekyll-TeXt-theme/docs/en/writing-posts)
- [Additional styles](https://tianqi.name/jekyll-TeXt-theme/docs/en/additional-styles)
- [Extensions](https://tianqi.name/jekyll-TeXt-theme/docs/en/extensions)
- [Markdown Enhancements](https://tianqi.name/jekyll-TeXt-theme/docs/en/markdown-enhancements)

## Demo Pages

| Name | Description |
| --- | --- |
| [Home](https://tianqi.name/jekyll-TeXt-theme/test/) | Home page |
| [Archive](https://tianqi.name/jekyll-TeXt-theme/archive.html) | Archive page |
| [Layout Examples](https://tianqi.name/jekyll-TeXt-theme/samples.html) | Examples for different layouts |

## License

TeXt Theme is [MIT licensed](https://github.com/kitian616/jekyll-TeXt-theme/blob/master/LICENSE).
