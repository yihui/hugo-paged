---
title: Getting started
author: Yihui Xie
categories:
  - Example
tags:
  - Tutorial
  - blogdown
  - Hugo
weight: 2
---

There are two ways to get started with this theme, depending on whether you use R or Hugo.

## R users

If you use R, the easiest way to get started is to install [the **blogdown** package](https://github.com/rstudio/blogdown), and create a new site with this theme:

```r
install.packages('blogdown')
blogdown::new_site(theme = 'yihui/hugo-paged')
```

Or you can [create a new RStudio **blogdown** project](https://bookdown.org/yihui/blogdown/a-quick-example.html) (if you use RStudio) with the `yihui/hugo-paged` theme.

## Hugo users

1. Create a new Hugo site with `hugo new`.
1. [Download this theme from Github](https://github.com/yihui/hugo-paged/archive/refs/heads/main.zip) and unzip it to the `themes/hugo-paged` directory.
1. Move all content of the `exampleSite` directory in this theme to the root directory of the new site.
1. Run `hugo server` and start playing with the new site.
