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

## Editing

Open `index.html` and edit it. There is no generator, no npm, no build. Commit
and push, and GitHub Pages republishes within a minute.

The workout schedule is a block of `<article class="ao">` cards inside a
`<section class="dayblock" data-day="...">` per day. To change a workout, edit
its card. To add one, copy a neighbouring card. To retire an AO, delete it and
decrement the count in that day's filter button near the top.

## Contact

The contact link is a `mailto:` to `f3greensboro.itq@gmail.com`. Because that
address is in public HTML it will attract spam. If that becomes a problem,
replace it with a Formspree form (free tier, no address exposed in the page).

## History

This replaced a WordPress site hosted on SiteGround, cancelled at the October
2026 renewal. The 4,998 backblasts posted there between 2014 and 2026 are
preserved as markdown in the private archive repository. New backblasts are
posted to PAX Vault in Slack, not here.
