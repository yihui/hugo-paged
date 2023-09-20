---
title: A Plain Markdown Post
subtitle: with a subtitle...
author: Yihui Xie
date: '2016-02-14'
categories:
  - Example
  - Hugo
tags:
  - blogdown
  - Markdown
  - KaTeX
  - Pandoc
  - RStudio
---

## Sample Text

### Third-level header

#### Fourth-level header

A paragraph (with a footnote):

**Lorem ipsum** dolor sit amet, consectetur adipiscing elit, sed do eiusmod
tempor incididunt ut labore et dolore *magna aliqua*. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident,
sunt in culpa qui officia deserunt mollit anim id est laborum.[^1]

[^1]: I'm sure you are bored by the text here.

\* \* \*

A blockquote (a gray bar at the left and lightgray background):

> Quisque mattis volutpat lorem vitae feugiat. Praesent porta est quis porta
> imperdiet. Aenean porta, mi non cursus volutpat, mi est mollis libero, id
> suscipit orci urna a augue. In fringilla euismod lacus, vitae tristique massa
> ultricies vitae. Mauris accumsan ligula tristique, viverra nulla sed, porta
> sapien. Vestibulum facilisis nec nisl blandit convallis. Maecenas venenatis
> porta malesuada. Ut ac erat tortor. Orci varius natoque penatibus et magnis
> dis parturient montes, nascetur ridiculus mus. Nulla sodales quam sit amet
> tincidunt egestas. In et turpis at orci vestibulum ullamcorper. Aliquam sed
> ante libero. Sed hendrerit arcu lacus.
>
> --- by Someone

A full-width piece of syntax-highlighted code with a drop-shadow effect:

``` js
// right-align a quote footer if it starts with ---
[...document.getElementsByTagName('blockquote')].forEach(quote => {
  const el = quote.lastElementChild;
  if (el?.tagName === 'P' && /^(—|---)/.test(el.textContent)) el.style.textAlign = 'right';
});
```

A full-width table:

| Sepal.Length | Sepal.Width | Petal.Length | Petal.Width | Species |
|-------------:|------------:|-------------:|------------:|:--------|
|          5.1 |         3.5 |          1.4 |         0.2 | setosa  |
|          4.9 |         3.0 |          1.4 |         0.2 | setosa  |
|          4.7 |         3.2 |          1.3 |         0.2 | setosa  |
|          4.6 |         3.1 |          1.5 |         0.2 | setosa  |
|          5.0 |         3.6 |          1.4 |         0.2 | setosa  |
|          5.4 |         3.9 |          1.7 |         0.4 | setosa  |

An image (automatically centered):

![Happy Elmo](https://slides.yihui.org/gif/happy-elmo.gif)

A math equation (render by KaTeX):

`$$|x| = \begin{cases} x & \text{if } x \geq 0 \\ -x & \text{if } x < 0  \end{cases}$$`

How about `Ctrl + C` and `Ctrl + V`?

## Another Section

Looks good?

Hope you will enjoy it.
