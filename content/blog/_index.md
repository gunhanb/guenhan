---
title: Blog
description: |
  A blog about biostats. I blog about what I found interesting in biostats/epidemiology and #rstats.
author: "Burak Kürsad Günhan"
show_post_thumbnail: true
thumbnail_left: false
show_author_byline: true
show_post_date: true
# for listing page layout
layout: list-sidebar # list, list-sidebar, list-grid

# for list-sidebar layout
sidebar: 
  title: Blog
  description:  
  author: "Burak Kürsad Günhan"
  text_link_label: Subscribe via RSS
  text_link_url: /index.xml
  show_sidebar_adunit: true # show ad container

# set up common front matter for all pages inside blog/
cascade:
  author: "Burak Kürsad Günhan"
  show_author_byline: true
  show_post_date: true
  show_comments: true # see site config to choose Disqus or Utterances
  # for single-sidebar layout
  sidebar:
    text_link_label: View recent posts
    text_link_url: /blog/
    show_sidebar_adunit: false # show ad container
---

** No content below YAML for the blog _index. This file provides front matter for the listing page layout and sidebar content. It is also a branch bundle, and all settings under `cascade` provide front matter for all pages inside blog/. You may still override any of these by changing them in a page's front matter.**