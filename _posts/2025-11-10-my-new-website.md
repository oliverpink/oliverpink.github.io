---
date: 2025-11-10 19:00:00 +0000
layout: post
title: "My New Website!"
description: "How I built a simple site with GitHub Pages and Jekyll."
image: /assets/img/mynewwebsite-hero.png
optimized_image: /assets/img/mynewwebsite-hero.png
tags: [website, blog, jekyll]
categories: general
author: oliverpink
---

Welcome! Here I share the steps I used to set up my own website for free using GitHub Pages and Jekyll. Now, this is not a tutorial, but this showcases what I did to get to this point.

## Why Jekyll + GitHub Pages?

In the past, I spent lots of time on website builders like Wix. Over time the UIs felt janky and overloaded, so building a small site with Jekyll turned out cleaner and faster for me.

You can build and publish a blog or portfolio for free, with simple tools and easy updates.

## Prerequisites

<table>
  <thead>
    <tr>
      <th>Prerequisites</th>
      <th>Version</th>
      <th>Information</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Ruby</td>
      <td>3.3.10 (2025‑10‑23)</td>
      <td>Required runtime for Jekyll.</td>
    </tr>
    <tr>
      <td>RubyGems</td>
      <td>3.5.22</td>
      <td>Ruby package manager used by Jekyll.</td>
    </tr>
    <tr>
      <td>Git for Windows</td>
      <td>2.51.2</td>
      <td>Recommended for version control and GitHub workflows.</td>
    </tr>
    <tr>
      <td>Jekyll</td>
      <td>4.4.1</td>
      <td>Static site generator that powers GitHub Pages.</td>
    </tr>
    <tr>
      <td>Bundler</td>
      <td>2.7.2</td>
      <td>Keeps gem versions consistent across environments.</td>
    </tr>
  </tbody>
  <tfoot>
  </tfoot>
</table>

For Jekyll on Windows, PowerShell may block gem installs until you change execution policy:

```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

# Heading 1


## Heading 2


### Heading 3


#### Heading 4

--page-break--



## Code


Cum sociis natoque penatibus et magnis dis `code element` montes, nascetur ridiculus mus.


```js


Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");


Call the function
adder(2, 6);
> 8
```


## Main Steps
- Sign up for GitHub
- Create a new repository
- Add your Jekyll site files, including `_config.yml` for config and `_posts/` for articles
- Enable GitHub Pages in the repo's Settings
- Your site deploys at `https://yourusername.github.io`

## Images
Add images with Markdown:

![My site screenshot](/assets/img/Screenshot 2025-11-10 at 19-26-15 Jekflix A blog theme for Jekyll.png "Example image")


## Lists
- It's free
- You own your content
- No need for paid hosting

## Wrap-Up
That's it! You now have a simple, personal website.

---

**How to use:**
- Save your post in the `_posts/` folder as `YYYY-MM-DD-title.md`.
- Match the title, description, date, and tags to your own content.
- Preview locally, then push to GitHub to publish.

If you want more advanced features (like tables, video, code, thumbnails), you can add them as needed. For most posts, stick to concise front matter and clear Markdown.[1][2][8]

---

If you'd like to see how to use categories or custom variables, or need help formatting images/tables, just ask for a specific example.