---
layout: post
title: "How I Set Up This Site with Jekyll & GitHub Pages"
date: 2026-03-02
tags: [tutorial]
subtitle: "A quick walkthrough for anyone wanting to do the same."
---

Setting up a personal site shouldn't be complicated. Here's how I built this one using Jekyll and GitHub Pages — completely free.

## Step 1: Create the repository

On GitHub, create a new repo named `yourusername.github.io`. This special naming convention tells GitHub to serve it as a website automatically.

## Step 2: Set up Jekyll locally

First, make sure you have Ruby installed. Then:

```bash
gem install bundler jekyll
cd your-repo
bundle install
```

## Step 3: Run locally

```bash
bundle exec jekyll serve
```

Open `http://localhost:4000` and you should see your site.

## Step 4: Write your first post

Create a file in `_posts/` following the naming convention:

```
YYYY-MM-DD-your-post-title.md
```

Add some front matter at the top:

```yaml
---
layout: post
title: "Your Post Title"
date: 2026-03-02
tags: [your-tag]
---
```

Then write your content in Markdown below.

## Step 5: Deploy

Just push to `main` and GitHub handles the rest. Your site will be live at `https://yourusername.github.io` within a couple of minutes.

That's it — a blog up and running in under 15 minutes!
