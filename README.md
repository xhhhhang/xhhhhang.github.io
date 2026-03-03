# Liu Renhang — Personal Site & Blog

A modern, colorful personal website and blog built with Jekyll, hosted on GitHub Pages.

## Quick Start

### 1. Create your GitHub repository

Go to GitHub and create a new repo named `yourusername.github.io` (replace `yourusername` with your actual GitHub username).

### 2. Push this project to your repo

```bash
cd jekyll-site
git init
git add .
git commit -m "Initial commit: Jekyll site"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

Go to your repo on GitHub → **Settings** → **Pages** → set source to `main` branch → Save.

Your site will be live at `https://yourusername.github.io` within a few minutes!

### 4. (Optional) Run locally

```bash
# Install Ruby and Bundler if you haven't already
gem install bundler

# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve
```

Visit `http://localhost:4000` to preview your site.

## Writing Blog Posts

Create a new Markdown file in `_posts/` with this naming format:

```
YYYY-MM-DD-your-post-title.md
```

Add front matter at the top:

```yaml
---
layout: post
title: "Your Post Title"
date: 2026-03-03
tags: [tag1, tag2]
subtitle: "Optional subtitle"
---

Your content here in Markdown...
```

## Customization

- **Site info**: Edit `_config.yml` (title, description, author, URL)
- **Styling**: Edit `assets/css/style.css` (colors are CSS variables at the top)
- **Navigation**: Edit `_layouts/default.html`
- **About page**: Edit `about.md`
- **Footer links**: Edit the footer in `_layouts/default.html`

## Project Structure

```
├── _config.yml          # Site configuration
├── _layouts/
│   ├── default.html     # Base layout (nav + footer)
│   ├── post.html        # Blog post layout
│   └── page.html        # Static page layout
├── _posts/              # Blog posts (Markdown)
├── assets/css/
│   └── style.css        # All styles
├── index.html           # Homepage
├── blog.html            # Blog listing page
├── about.md             # About page
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```
