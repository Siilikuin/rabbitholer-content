---
title: "Welcome to Rabbitholer"
subtitle: "Turn an unordered set of Markdown files into a plain HTML website."
date: 2024-06-02
tags:
- rabbitholer
- example
---


Because WordPress is just too darn complicated.

**Rabbitholer** is a project with a simple goal: Leverage the power of
Git submodules to make it as simple as can be to generate a static
website from Markdown files, but no simpler.

What you are reading
right now is
[a properly-formatted example post from `rabbitholer-content`](https://github.com/Siilikuin/rabbitholer-content).

All your posts will need at least a `title` tag. You may also want

- A `subtitle` tag,
- A `date` tag, in `YYYY-MM-DD` format, and
- a set of `tags` to aid future navigators.

After that, you can put in whatever Markdown you want!

Once you're ready, simply fork
[the `rabbitholer` repo](https://github.com/Siilikuin/rabbitholer)
itself and add your `rabbitholer-content` as a Git submodule,
into the `content/` repo. And, presto - you now have a fully-functioning
Hugo website, complete with a sitemap and index page, you can
run locally with

```bash
hugo server
```

and deploy easily to Github Pages. No sweat!
