
# College Fest Website

This project implements the **Tuesday Scenario: College Fest Website**.

## What’s included
- A single-page site (`index.html`) with:
  - **Schedule**: an HTML `<table>` listing events, dates and timings.
  - **Gallery**: at least three images using `<figure>` and `<figcaption>`.
- Basic responsive design, accessible markup, and styled buttons.
- Three local placeholder images in `assets/images/`.

## How to run
Open `index.html` in any browser.

## Git workflow per instructions

```bash
# 1) Initialize repo
git init
git add .
git commit -m "chore: base project scaffold"

# 2) feature/schedule branch – add the schedule table
git checkout -b feature/schedule
# (In this project, the schedule table already exists in index.html)
git add index.html
git commit -m "feat(schedule): add events table to index.html"

# 3) feature/gallery branch – add the image gallery
git checkout main
git checkout -b feature/gallery
# (In this project, the gallery and images are already present)
git add index.html assets/images/*
git commit -m "feat(gallery): add gallery section with figure and figcaption"

# 4) Merge both features into main
git checkout main
git merge feature/schedule --no-ff -m "merge: schedule into main"
git merge feature/gallery --no-ff -m "merge: gallery into main"

# 5) Create GitHub repo and push
# Replace YOUR-REMOTE-URL with your GitHub repo URL (e.g., git@github.com:user/college-fest-website.git)
git remote add origin YOUR-REMOTE-URL
git branch -M main
git push -u origin main
```

> If you want to strictly simulate adding content only inside each feature branch,
> you can start with a minimal `index.html` on `main`, then add the table on
> `feature/schedule`, and add the gallery on `feature/gallery`, finally merging both.
> The end result should match the `index.html` in this project.
```

