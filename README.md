# Stephenson Ranch Cabins Website

This is the source for stephensonranch.com — a simple one-page site with a "Book on Airbnb" button for each cabin.

## Editing the site

Everything is in one file: `index.html`. All the text, colors, and layout live in there (the styling is in the `<style>` block near the top). To change any wording, find the matching text in the file and edit it directly — no build step, no command line needed.

## Swapping or adding photos

The `images/` folder already has real photos wired up. To replace one, upload a new file with the *same name* (GitHub will ask "replace this file?" — say yes) and the site updates automatically. Current filenames and what uses them:

- `hero.jpg` — big banner photo at the top of the page
- `old-cabin.jpg` — photo on The Old Cabin's card
- `hoover-cabin.jpg` — photo on The Hoover Cabin's card
- `story-creek.jpg` — photo inside the "Highwood Mountains" story section
- `og-cover.jpg` — the image shown when the link is shared on Facebook/Instagram (keep this one roughly 1200×630px, landscape)
- `gallery-trail.jpg`, `gallery-road.jpg`, `gallery-meadow.jpg`, `gallery-creek.jpg` — the four-photo strip below "Plan Your Stay"

To add a *new* photo (not replacing one of the above), upload it to `images/` with any name, then in `index.html` add a line like `<img src="images/your-filename.jpg" alt="describe the photo">` wherever you want it to show up.

Photos should be JPG or PNG, not HEIC (iPhone's default format) — most browsers can't display HEIC. On iPhone: Settings → Camera → Formats → "Most Compatible" makes future photos save as JPG automatically. To convert existing HEIC photos, open them in the Photos app and use Share → any option other than "Options: HEIC keeps original" (or ask me — I can convert a batch for you anytime).

## Publishing changes

Any change pushed to the `main` branch automatically updates the live site within a minute or two, since this repo is connected to GitHub Pages.
