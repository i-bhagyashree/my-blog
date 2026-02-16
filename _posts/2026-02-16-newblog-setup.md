---
layout: post
title:  "Building My Second Blog: A Jekyll Setup Story"
date:   2026-02-16 13:19:52 +0530
categories: learning-by-doing
description: "My journey of setting up a second Jekyll blog and publishing it to GitHub Pages."
---

I created my first Jekyll blog and wanted to publish it to GitHub Pages. First I initialized a local git repository and prepared my files:

```bash
git init
git add .
git commit -m "Initial commit"
```

Then I created a new repository on GitHub, linked it to my local repo, and pushed:

```bash
git remote add origin https://github.com/your-username/myblog.git
git push -u origin main
```

When I opened GitHub Pages, it showed an error. I fixed the site URL and re-committed the change:

```bash
git add *
git commit -m "Update site URL"
git push
```

I also discovered a repository-name issue: I had used `Myblog` locally but the correct repository name on GitHub was `myblog` (lowercase). After renaming to match and pushing again, the site published successfully.

These small fixes—correcting the URL and matching the repository name—resolved the publishing errors. Now the blog is live and I can continue writing and sharing what I learn.

## Committing Changes

After making changes (for example, updating `_config.yml`, fixing the site URL, or renaming files), use these commands to review, commit, and push your updates:

```bash
# See what changed
git status

# Review differences (optional)
git diff

# Stage all changes
git add .

# Commit with a clear message
git commit -m "Fix site URL and repository name"

# Push to the remote branch
git push
```

If you need to push to a specific branch (e.g., `main`), use `git push origin main`.
