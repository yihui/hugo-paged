---
title: Customization
author: Yihui Xie
categories:
  - Example
tags:
  - Tutorial
weight: 3
---

The more you know, the less real work you will get done. You have been warned.

## Site config

In your site config file (`hugo.yaml` or `config.yaml`), you can customize some options such as the top menu or footer, which should be straightforward to understand if you take a look at the `exampleSite`'s config file.

If you want to add a logo to the left of the top navigation bar, you can use the `logo` parameter, e.g.,

```yaml
params:
  logo:
    en:
      alt: "LOGO TEXT"
      img: # a path to the logo
```

If the image (`img`) is not provided, the `alt` text will be displayed instead.

## CSS

You can create a file `static/css/custom.css` to store your custom CSS code. For example, if you don't like code blocks to be full-width, you can reset their width:

```css
@media (min-width: 992px) {
  .main > pre {
    width: 100%;
    margin-left: auto;
  }
}
```

### Dingbats

If you want to choose a different symbol such as a snow flake to be placed behind the page title, you can define the CSS:

```css
.title::before { content: "❆"; }
```

<style type="text/css">
.title::before {
  content: "❆";
}
</style>

Any character that can be displayed in your web browser is okay. For example, you can choose one dingbat from <https://en.wikipedia.org/wiki/Dingbat>.

<div style="font-size:9em;color:#ddd;text-align:justify;max-height:5em;overflow-y:scroll;">
✁	✂	✃	✄	✆	✇	✈	✉	✎	✏ ✐	✑	✒	✓	✔	✕	✖	✗	✘	✙	✚	✛	✜	✝	✞	✟ ✠	✡	✢	✣	✤	✥	✦	✧	✩	✪	✫	✬	✭	✮	✯ ✰	✱	✲	✳	✴	✵	✶	✷	✸	✹	✺	✻	✼	✽	✾	✿ ❀	❁	❂	❃	❄	❅	❆	❇	❈	❉	❊	❋	❍	❏ ❐	❑	❒	❔	❕	❖	❘	❙	❚	❛	❜	❝	❞		❡	❢	❣	❤	❥	❦	❧	❨	❩	❪	❫	❬	❭	❮	❯ ❰	❱	❲	❳	❴	❵ ➔	 ➘	➙	➚	➛	➜	➝	➞	➟ ➠	➡	➢	➣	➤	➥	➦	➧	➨	➩	➪	➫	➬	➭	➮	➯	➱	➲	➳	➴	➵	➶	➷	➸	➹	➺	➻	➼	➽	➾
</div>

### Sticky menu

It's easy to make the top menu sticky if you desire:

```css
.nav-top {
  position: sticky;
  top: 0;
  background-color: white;
}
```

### Typefaces

If you don't like the default typefaces of this theme, you can create `static/css/fonts.css` to override them.

## Templates

As the last (and most powerful) resort, you can always override the template files under `layouts/`. I don't really have enough time to document everything. Please try to help yourself.
