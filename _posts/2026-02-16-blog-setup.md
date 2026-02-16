---
layout: post
title:  "Building My First Blog: A Jekyll Setup Story"
date:   2026-02-16 13:19:52 +0530
categories: learning-by-doing
description: "My journey of setting up a Jekyll blog from scratch, including debugging issues and upgrading Ruby."
---

## Why I Started This Blog

I created this blog to document my learning journey—to capture the errors I encounter, the solutions I discover, and the new technologies I explore. It's my personal learning journal where I can look back and remember what I learned and how I solved problems along the way.

## The First Challenge: VS Code Debugger

While working on a project today, I hit my first hurdle. I tried running my code through the VS Code run bar, but kept getting an error popup about debugging. I realized the issue: I didn't have a debugger installed on my system. 

**The fix:** I switched to the "Run Code" option in VS Code it was throwing an error because of misconfigured json file which i was not able to figure it out so i asked copilot for help it fixed the files for me and installed the necessary debugger & Problem solved!

## Setting Up Jekyll: The Main Task

Inspired by this experience, I decided to create a blog using Jekyll to share what I learn. Here's the step-by-step process I followed:

### Step 1: Upgrade Ruby

Jekyll requires a modern version of Ruby. My system had an older version, so I needed to upgrade it.

```bash
# Update brew
brew update
brew install rbenv ruby-build

# Initialize rbenv
rbenv init

# Install the latest Ruby version
rbenv install -l
rbenv install 3.4.1

# Set it as the global version
rbenv global 3.4.1

# Verify the upgrade
ruby -v
```

### Step 2: Install Jekyll and Bundler

```bash
gem install jekyll bundler
```

### Step 3: Create a New Jekyll Site

```bash
jekyll new myblog
cd myblog
```

### Step 4: Build and Run Locally

```bash
bundle exec jekyll serve
```

## The Result

After running these commands, my blog was live! I renamed it to "Learning by Doing" to reflect my mission, updated my configuration with my details, and published my first post documenting today's learnings and challenges.

This blog is now my space to share what I'm learning, the technologies I'm exploring, and the interesting things I discover—hopefully inspiring others who are curious about tech.
