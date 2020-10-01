# Onshape4FRC

Built using the [mediumish](https://github.com/wowthemesnet/mediumish-theme-jekyll) jekyll theme


## Settting up your development enviornment

1. Follow the guide to the install jekyll for your operating system type
   - https://jekyllrb.com/docs/installation/
2. Clone this repo to your local machine
   - If you're new to git the easiest way is probably [Github Desktop](https://desktop.github.com/)
3. Open the folder where you cloned this repo in your favorite editor (I suggest VSCode and will be refering on how to do things in the future using it)
4. Open a new terminal at this folder (This can be done with Terminal -> New Terminal in VSCode)
5. Run `bundle exec jekyll serve` to start up the server
   - Most likely it will serve on 'localhost:4000'


## Making changes

All changes should be tested locally by running the local server and checking them in the browser. This allows for quickly previewing changes. Once you push them to the master branch of git they will be built and pushed to live on the site. 

**Common Data**

Common data is stored in the `_data` directory. This is information which is either very repeated or used in multiple places. So far this is the information about blog authors and the featurescript list, but there's no reason more can't be stored here as needed. You can view how to use this data on [this page](https://jekyllrb.com/docs/datafiles/) or by looking in the code for a previous example. 

**Assets**

All assents (images, CSS, JS, Fonts) are stored in this folder. When placing images try to keep them organized in folders based on where they're used. For example put blog images in the blog folder, then a sub folder for the particular post you're making.

**Pages**

The base pages are stored in the `_pages` directory. These are written in a mix of HTML and markdown and the layout is powered by bootstrap. They also take advantage of the liquid library for HTML generation. 

**Blog**

To add a new post to the blog simply create a new markdown file in the `_posts` directory. It must follow the format `YYYY-MM-DD-url-of-post.md`. The date is the date this post was made on and the rest of the name is the url this post will live at. 

The file needs a header at the top which contains some data about the post, an example of which is below. The author must be present in the `_data/authors.yml` file. Categories can be anything you want but should be standard across posts. By default set `featured` and `hidden` to false (featured will put the post in the featured section on the homepage and the top of the blog page).

```
---
layout: post
title: "Using the TubeConverter Featurescript"
author: max
categories: [Onshape, Featurescripts]
image: assets/images/blog/tubes.png
featured: true
hidden: false
comments: false
---
```

The posts can be written in any combination of markdown and HTML. Unless required to create multiple columns or an embedded video it is recommended to stick to pure markdown.