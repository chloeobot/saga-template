# Saga template

A Saga is your own written account of running apps on ElfHosted. You draft it with Sam, ElfHosted's assistant, publish it on your own GitHub Pages site, and earn hosting credit for it whatever it says. This template turns the files from your ElfBot Saga export into a clean, readable site.

## Set it up

1. Click **Use this template** at the top of this page, then **Create a new repository**. Make it public.
2. Replace the sample files with the files from your ElfBot Saga export, keeping the same names:
   - `index.md`
   - `_data/saga.yml`
   - `chapters/` (one file per chapter, named `YYYY-MM.md`)
   - `assets/` (your charts, as `.svg` files)

   Delete `chapters/2026-12.md` and `assets/sample-availability.svg` if your export doesn't replace them. Leave `assets/saga.css` and the `_layouts` folder alone.

   Your export may also include a `share/` folder of copies you can paste into other blogs and a `saga-drafts/` folder. This template never publishes either one, so they stay private even though they sit in your repository.
3. In your repository, go to **Settings**, then **Pages**. Under **Build and deploy**, choose **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, then save. Your site appears at `https://USERNAME.github.io/REPO` within a minute or two.

## Choose a look

Open `_data/saga.yml` and set two lines:

```
style: long-read
palette: forest
```

- `style` is `long-read` (an essay), `uptime-log` (a log of short entries with the chart up front) or `at-a-glance` (cards in a grid).
- `palette` is `forest`, `dusk`, `ember`, `tide` or `graphite`. Each one has a light and a dark version that follow the reader's device.

If a value is missing or misspelled, the site uses `long-read` and `forest`. Your `description` in the same file is what search engines and link previews show.

## Add a chapter

Create a file in `chapters/` named for the year and month, such as `chapters/2027-01.md`:

```
---
layout: chapter
title: "January 2027"
date: 2027-01-20
---

What happened this month.
```

It shows up in the chapter list on your Saga page, newest first. To use a chart, put an `.svg` file in `assets/` and add `![A short description](assets/name.svg)` to the chapter.

## Keep it pseudonymous

- Set `author` in `_data/saga.yml` to a pseudonym, or remove the line to show no name.
- Commits carry the git author name and email you used. Check them with `git config user.name` and `git config user.email`, and use a pseudonym and your GitHub noreply address if you want to stay private.
- Your GitHub profile and username are visible too. Check them before you share the link. Your username is part of the default site address.

## It's yours

The repository and the site belong to you. Edit the text freely, and delete the repository or turn off Pages at any time to take it down.

## The disclosure stays

Every page shows a short note that you received hosting credit and that your opinions are your own. It lives in `_layouts/default.html`, not in your content, so editing `index.md` or `saga.yml` doesn't change it. It has to stay in place for the reward.

## Licence

MIT. See `LICENSE`.
