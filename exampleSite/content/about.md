---
title: About Hugo Paged
subtitle: A theme that started with four crop marks in the corners
author: Yihui Xie
menu:
  main:
    name: About
    weight: 1
---

I immediately loved the design of [the paged.js website](https://pagedjs.org) when I first saw it a couple of years ago.[^1] I have published a few books before, so the crop marks on the website caught my attention first, which gave me a familiar feel of printed books. The second thing that I appreciated was the rotated floral heart bullet behind the title of each page, i.e.,

<div style="font-size:9em;text-align:center;color:#ccc;">❧</div>

So I wrote a Hugo theme that mimics the style of the paged.js website. I tried not to look at its HTML/CSS source code, but I had to read the source to figure out:

1. How the crop marks were made with CSS (a very clever trick that I'd never thought of);
1. What the floral heart symbol really was (I'd never know this dingbat);
1. The fonts ([Linden Hill](https://github.com/theleagueof/linden-hill) and [Jost](https://github.com/indestructible-type/Jost)).

The rest of HTML and CSS code was written from scratch (well, not really---from [the Hugo XMin theme](https://github.com/yihui/hugo-xmin)). The code is fairly lightweight and hopefully easy for users to understand, tweak, or adapt.

I'd like to thank paged.js developers for their great piece of work, without which I wouldn't be able to create this theme.

I hope this theme won't be widely known or used because I'm currently using it for my own website...[^2] but I'm all for open source, so [here you go](https://github.com/yihui/hugo-paged)! If you decide to use this theme, I encourage you to tweak the CSS to make your site look at least a little different.

[^1]: When I was developing [the **pagedown** package](https://github.com/rstudio/pagedown) in R.

[^2]: Paged.js developers are more generous than me. They were quite happy to know that I created this Hugo theme, and were not concerned that other websites would use their website theme. Hat tip to them!
