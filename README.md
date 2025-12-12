
Website for the **1st International Workshop on Causal Learning and Reasoning in Agents and Multi-Agent Systems (CLaRAMAS)** hosted by [AAMAS 2026](https://cyprusconferences.org/aamas2026/).

# Structure

Here are the main files of the template

```shell
./Type-on-Strap
├── _includes	               # Theme includes
├── _layouts                   # Theme layouts (see below for details)
├── _portfolio	               # Collection of articles for the portfolio page
├── _posts                     # Blog posts
├── _sass                      # Sass partials (compiled into css at runtime)
├── assets
|  ├── js	               # JS compiled for distribution + raw sources
|  ├── css                     # CSS compiled for distribution
|  ├── fonts		       # Font-Awesome, and other fonts
|  └── img		       # Images used for the template
├── pages
|   ├── 404.md		       # To be displayed when url is wrong
|   ├── about.md               # About example page
|   ├── gallery.md             # Gallery page for your photos
|   ├── portfolio.md	       # Portfolio page for your projects
|   ├── search.md	       # Search page
|   └── tags.md                # The tag page
├── _config.yml                # sample configuration
├── _data
|  ├── authors.yml             # Update the post authors configurations 
|  ├── comments.yml            # Comments configuration (Disqus, Cusdis, Utterances, Giscus)
|  ├── language.yml            # Localization configuration
|  ├── biblio.yml              # To create a reference bibliography
|  ├── social.yml              # Social configurations to share posts (RSS, shares, ...)
|  └── icons.yml               # Footer icons (Twitter, Github, Stackoverflow, ...)
└── index.html                 # sample home page (blog page paginated)
```

# Blogging

When writing a post, be sure in jekyll to:
 - Put it in the `_posts` folder
 - Name it with the date first like `2019-08-21-This-is-my-blog-post.md`

Please refer to the [Jekyll docs for writing posts](https://jekyllrb.com/docs/posts/). 

## Layout: Post

These are the basic features you can use with the `post` layout, in the comment the `Opt` means that
it is optional.

```yml

---
layout: post
title: Hello World                                # Title of the page
hide_title: true                                  # [Opt] Hide the title when displaying the post, but shown in lists of posts
feature-img: "assets/img/sample.png"              # [Opt] Add a feature-image to the post
thumbnail: "assets/img/thumbnails/sample-th.png"  # [Opt] Add a thumbnail image on blog view
color: rgb(80,140,22)                             # [Opt] Add the specified color as feature image and links in post
position: 1                                       # [Opt] Set position on the menu navigation bar
tags: [sample, markdown, html]                    # [Opt] Add tags to the page
---
```

With `thumbnail`, you can add a smaller image than the `feature-img`. 
If you don't have a thumbnail, you can still use the same image as the feature one. Or use the gulp task to create it.

If you don't use a feature image, but `color`, the transparent background is set comes from [`lineart.png`](assets/img/lineart.png). 
You can edit it in the config file (`_config.yml > color_image`). If you want another one, put it in `/assets/img` as well. 

For position, if not set on all pages, it will be by alphabetical order without `position` then by `position` order.
If two pages have the same position number, the order is decided by alphabetical order on the page title.

There's also `bootstrap: true` which is not mandatory and only useful if you want to add HTML content in your page that
requires [bootstrap](http://getbootstrap.com/).
It will respect the page and theme layout, mind the padding on the sides.

## Post excerpt

The [excerpt](https://jekyllrb.com/docs/posts/#post-excerpts) is the head of the article rendered in the blog page. 
The length of the excerpt has a default of around `250` characters or can be manually set in the post using:

in `conflig.yml`:

```yml
excerpt: true
```

Then in your post, add the `excerpt separator`:

```yml

---
layout: post
title: Sample Page
excerpt_separator: <!--more-->
---

some text in the excerpt
<!--more-->
... rest of the text not shown in the excerpt ...
```

The html is stripped out of the excerpt, so it only displays text.

## Image aligner

To easily add align images side by side in your article using the `aligner.html` include:

```liquid
{% include aligner.html 
  images="path/to/img1.png,path/to/img2.png,path/to/img3.png" 
  column=3 
  caption="some description" 
%}
```

Use it in any markdown file. There are two fields in the _include_ you need to look into:
  - _images_: Takes a string separated with `,` of all the images' path. 
    - It by default look into `assets/img/` so give the path from there.
  - _column_: (OPTIONAL) Set the number of column you want your imaged displayed in.
    - default is 2 columns
    - `column=3` set 3 columns
    - `column="auto"` makes as many columns as images
  - _caption_: (OPTIONAL) Add a caption to the images

## Code highlight

Like all CSS variables in the theme, you can edit the color of the code highlight in `_sass > base > _variables.scss`.
The code highlighting works with [base16](https://github.com/chriskempson/base16-html-previews/tree/master/css) you can find existing example 
of your favourite highlight color scheme on this format.

# This website is built with Type on Strap 🎨

[![Default Type on Strap blog](https://github.com/Sylhare/Type-on-Strap/blob/master/assets/img/screenshot.png?raw=true)](https://sylhare.github.io/Type-on-Strap/)

A free and open-source [Jekyll](https://jekyllrb.com) theme. 
Based on Rohan Chandra [type-theme](https://github.com/rohanchandra/type-theme) packed with extra features and easily customizable.

# Contact

[Stefano Mariani](https://smarianimore.github.io/)
