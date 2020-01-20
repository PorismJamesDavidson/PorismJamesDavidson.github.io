---
layout: default
title: Local install
permalink: /install/

---

# To serve site locally

## Using Ruby installer

[Follow instructions here](https://jekyllrb.com/docs/installation/windows/#installation-via-rubyinstaller)

After install:
`gem install jekyll -v 3.8.5` Use current version on [Github Pages](https://pages.github.com/versions/)

`gem install jekyll-theme-slate jekyll-paginate jekyll-sitemap jekyll-gist jekyll-feed jemoji jekyll-include-cache jekyll-relative-links wdm`

### To serve to localhost

`jekyll serve`

[127.0.0.1:4000](http://127.0.0.1:4000/)

## Using ubuntu or Linux sub-system for window ubuntu.

### To install

`sudo apt-get update -y && sudo apt-get upgrade -y`  
  
`sudo apt-add-repository ppa:brightbox/ruby-ng`
  
`sudo apt-get update`

`sudo apt-get install ruby2.5 ruby2.5-dev build-essential dh-autoreconf zlib1g-dev`

`sudo gem update`

`sudo gem install jekyll -v 3.8.5` Use current version on [Github Pages](https://pages.github.com/versions/)

`sudo gem install jekyll-theme-slate jekyll-paginate jekyll-sitemap jekyll-gist jekyll-feed jemoji jekyll-include-cache jekyll-relative-links`

### To serve to localhost

`jekyll serve`

[127.0.0.1:4000](http://127.0.0.1:4000/)
