# f3greensboro.com

The public F3 Greensboro website. Served by GitHub Pages straight from `main`.

**This repository is public.** Everything committed here is visible to anyone on
the internet, forever, including after it is deleted. Do not put the backblast
archive, the member roster, the WordPress export, or anything containing real
names or email addresses in this repository. Those live in the private
`f3greensboro` repository and must stay there.

## What's here

| File | What it is |
|---|---|
| `index.html` | The entire website. One page, no build step, styles inline. |
| `404.html` | Shown for any old WordPress URL. Points people at PAX Vault. |
| `photos/` | Photos for the top of the page. See **Photos** below. |

## Editing

Open `index.html` and edit it. There is no generator, no npm, no build. Commit
and push, and GitHub Pages republishes within a minute.

The workout schedule is a block of `<article class="ao">` cards inside a
`<section class="dayblock" data-day="...">` per day. To change a workout, edit
its card. To add one, copy a neighbouring card. To retire an AO, delete it and
decrement the count in that day's filter button near the top.

## Photos

The top of the page shows one photo from `photos/`, picked at random on each
visit. The list of photos is in `index.html`, in the script just under the
headline, one line per photo with its size, alt text, caption and focal point.

To add one:

1. Resize it to about 1600px on the long side, 200-400 KB. Phone originals are
   several megabytes and would make the page slow on mobile data.
2. Strip its metadata (location, camera, date) — `exiftool -all= photo.jpg`.
3. Put it in `photos/` and add a line to the list in `index.html`.

Put full-size originals in `photos/originals/`. That folder is git-ignored, so
they never reach this public repository. Only use photos the men in them are
fine being on a public website with, and no children.

## Contact

The contact button points at a Google Form owned by the `f3greensboro.itq@gmail.com`
account: https://forms.gle/hmx6kDfQBexPRHHz5

It lives on that account deliberately. Whoever inherits the ITQ inbox inherits the
form, its responses and its notifications — there is no separate vendor account to
hand over. If responses ever stop arriving, check **Responses → ⋮ → Get email
notifications for new responses** on the form; the old WordPress contact form
failed silently for years and nobody noticed.

The email address is also offered as a fallback, but it is assembled by JavaScript
at the bottom of `index.html` rather than written into the page, so address
harvesters scraping the HTML find nothing. If you edit that block, keep it that way.

## History

This replaced a WordPress site hosted on SiteGround, cancelled at the October
2026 renewal. The 4,998 backblasts posted there between 2014 and 2026 are
preserved as markdown in the private archive repository. New backblasts are
posted to PAX Vault in Slack, not here.
