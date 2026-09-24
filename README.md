# sandhills-guest-page

**Machine-generated. Public on purpose. Do not put anything private here.**

`page.html` is the weekly "What's On This Week" listing for
[visitpinehurst.com](https://visitpinehurst.com), written every Sunday morning by the
`sandhills-guest-brief` routine and read by the **Sandhills Week** WordPress plugin over plain
HTTPS:

```
https://raw.githubusercontent.com/cxm5267-crypto/sandhills-guest-page/main/page.html
```

This repo exists only so the website can fetch that file without credentials. Nothing
authenticates to WordPress, and WordPress authenticates to nothing — it just reads a public URL
and caches the result.

## What's in page.html

A fortnight of days, each one a section tagged with its date:

```html
<section class="sw-day" data-date="2026-09-28">
  <h3>Monday, September 28</h3>
  <ul><li><strong>Event</strong> — 7pm, Venue, Southern Pines. $15.</li></ul>
</section>
```

The plugin drops days that have passed and renders the next seven, which is what lets one weekly
run read as a rolling week. It also fetches the forecast from the National Weather Service
itself, so there is deliberately no weather table in this file.

## Source

Everything that generates this — the prompt, the local knowledge, the checks and the plugin —
lives in the private `sandhills-guest-brief` repo. Edit it there, never here: anything committed
to this repo by hand is overwritten on the next Sunday run.
