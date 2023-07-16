## Anope Site

This repository contains the Jekyll sources for the Anope Website. Changes that are pushed to this repository are automatically deployed to GitHub Pages.

### Making a News Post

To make a new news post:

- Create a file in `_posts` with a name like `2020-04-20-hello-world.md`
- Edit the following front matter and add it to the top of the page:

```yaml
---
layout: post
title: Post Title
author: Your Name
category: Current Year (e.g. 2010)
---
```

- Write your post after the front matter
- Commit your changes
- Push to GitHub

The site will be automatically rebuilt and will show your post as the most recent one. If you're not sure about anything check some older posts to see how they do it but be aware that posts from before the Jekyll migration use a lot of raw HTML instead of Markdown and may not be formatted as well as they could.

If your post is particularly long and you don't want to show the whole thing on the news index you can add a comment like `<!--more-->` to hide all contents after it.
