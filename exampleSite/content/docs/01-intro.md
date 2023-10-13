---
title: Introduction
author: Yihui Xie
categories:
  - Example
  - Hugo
weight: 1
---

The Hugo Paged theme was inspired by [the paged.js website](https://pagedjs.org).

## The paged.js website

The paged.js library is awesome. Its website is also beautiful.

### The crop marks

I love the crop marks. I couldn't imagine that they were made from three rectangles:

```html
<div class="crop-h"></div> <!-- horizontal lines -->
<div class="crop-v"></div> <!-- vertical lines -->
<div class="crop-c"></div> <!-- cover some segments -->
```

Make their position absolute, and shrink them a little bit:

```css
.crop-h, .crop-v, .crop-c {
  position: absolute;
  z-index: -1;
}
.crop-h {
  inset: 2em 0;
  border-top: 1px solid;
  border-bottom: 1px solid;
}
.crop-v {
  inset: 0 2em;
  border-left: 1px solid;
  border-right: 1px solid;
}
.crop-c {
  inset: 1em;
  border: 1.5em solid white;
}
```

Isn't that clever? Thank you, paged.js developers!

### The floral heart

I also love the floral heart behind the title of each page, which is a dingbat:

```css
h1.title::before {
  content: "❧";
}
```

## Making a Hugo theme

Once I understood the above tricks, I developed a Hugo theme based on my previous [Hugo XMin theme](https://github.com/yihui/hugo-xmin). This theme is still very lightweight. The total number of lines of CSS is about 240.

## Blog and/or documentation

This theme supports two types of lists of pages: [blog](/blog/) and [documentation](/docs/).

- A blog list shows the post summaries in the list. You can either define a post summary via the `description` field in the YAML metadata of a post, or let this theme generate an automatic summary from the paragraphs of your post.
- A documentation list shows the tables of contents of documentation pages. This is similar to the table of contents of a book, so you could use this theme to write a book (or two).

By default, pages under the `content/blog` directory will use the blog list, and pages under `content/docs` will use the documentation list. If you want other pages to use the `blog` or `docs` list layout, you can specify the `layout` field in the YAML metadata of `_index.md` (e.g., `layout: docs` in `content/foo/_index.md`).

If you want to order pages manually in the list, you can set the `weight` field in the YAML metadata of pages.
