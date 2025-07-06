---
title: My First Post
slug: my-first-post
description: 
tags: 
date: 2025-07-06T03:00:00+05:00
draft: false
image: 
layout: 
excludeSearch: false
unlisted: false
toc: false
---
FINALLY got my blog set up. Shifted between 5 different themes and finally decided on this one (thank you Nick for the [insightful tutorial](https://www.nickgracilla.com/posts/obsidian-is-my-hugo-cms/)).

Anways,

<style>
.responsive-image-container {
  max-width: 300px;
  width: 100%;
}

.responsive-image-container img {
  width: 100%;
  height: auto;
  max-width: 300px;
}

/* Mobile: image at top */
@media (max-width: 768px) {
  .content-wrapper {
    display: flex;
    flex-direction: column;
  }
  
  .responsive-image-container {
    order: -1;
    margin: 0 auto 20px auto;
    text-align: center;
  }
  
  .main-content {
    order: 1;
  }
}

/* Desktop: image beside text */
@media (min-width: 769px) {
  .content-wrapper {
    display: flex;
    flex-direction: row;
    gap: 20px;
    align-items: flex-start;
  }
  
  .main-content {
    flex: 1;
  }
  
  .responsive-image-container {
    flex-shrink: 0;
    margin: 0;
  }
}
</style>

<div class="content-wrapper">
<div class="main-content">

# Hello.
The purpose of this blog is to just document random stuff that I keep getting myself into and eventually forget what I did. And also to just show random projects that I take on (which is directly proportional to the free time that I have)

You will hear more from me. Soon.

</div>

<div class="responsive-image-container">
<figure>
<img src="my-notion-face-transparent.png" alt="My Notion avatar">
<figcaption>me sorta kinda as a Notion avatar</figcaption>
</figure>
</div>

</div> 