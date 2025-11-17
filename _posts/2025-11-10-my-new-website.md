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

For Jekyll on Windows, it block gem installs until you change the execution policy in Powershell using the first command. You can re-enable this policy using the second command:

```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned

Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Restricted
```

# Tutorial

I used the first part of the video to create my website. As I used a different template to his, I used Perplexity AI to figure out how to change the values to my liking. 

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/g6AJ9qPPoyc?si=Eikhkt1phJ2-AxpM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Template

I used the template named <a href="https://github.com/thiagorossener/jekflix-template">Jekflix</a>. Looks like Netflix (duh), but it also has everything I want on a website.


## Cloning

After forking the project to your github, you can clone your project and locally host it. Typically, it would be stored within your git folder, so whether you have git as a program or as a portable application, it should be within that folder.

## Referencing your project in Git

1. Open your Git Terminal
2. Type in ```cd (project directory)```. <br>For me, this was ```cd /g/programs/portablegit/oliverpink.github.io```. This connects your Git terminal to your git project.

After this, there are many commands you can do. For my instance, it would be locally hosting and uploading it live to your website.

### Local Host

Type this command:
```
bundle exec jekyll serve 
```
This will boot up a local server, given that there are no errors. It's also a good way to check if your images are directed correctly as each time you refresh, it'll respond with a good ERROR message.

To see your website, connect to <a href="localhost:4000">localhost:4000</a> in your browser.

To stop your local build, go back to your Git Terminal and CTRL + C and terminate batch job.

Additionally, if your changes aren't seen in your local build, you can use `bundle exec jekyll clean` to refresh the site's local files, which are built every run. You can also combine this with jekyll serve so you don't have to do two commands every time:
```
bundle exec jekyll clean  && bundle exec jekyll serve
```

### Upload to Live Build

Type these commands:
```
git add .
git ad commit -m "(notes here)
git push origin main
```
Couple of notes:
- If the project branch in your project pages tab is set as master, replace main as master. If it is named main, do not change. 
- If remote is not set up, use ```git remote add origin https://github.com/yourusername/yourusername.github.io.git```


### Updating the Config file

In the Jekflix template, there is a `config.yml` file to control things like:
- Website Name
- Website Title
- Website Description 
- Tags
- Menu pages
- Email
- Contact Form Setup
- Social Media Settings (enable/disable social media buttons)
- Post settings
- URL & Language
- Google Analytics/SEO
- How the website will function (paginators, builds and miscellaneous back-end things)
- & more

## Creating New Posts


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