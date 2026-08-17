# snowball-website

Source for www.snowball-consult.com. Static single-page site, no build step: edit `index.html`, push, live.

## Status

Front page (`index.html`) is a minimal widget: logo, one-liner, and a Claude Code-style
status spinner cycling through 200 consulting/GTM-ops terms (Esc or click "interrupts" it).
The full Andreas-dictated landing copy lives on at `about.html`, linked from the footer;
the dictation source with cleanup notes lives in the `claude` repo at
`snowball-service-offering/website/2026-08-17_dictated-landing-copy-picking-the-right-problem.md`.
Purpose of the site: digital footprint plus a decent understanding of which type of problem
Snowball Consult solves. Planned later: blog and resources sections.

## Design

Deliberately minimal and text-first: single column on FT paper `#FFF1E5`, Newsreader serif
for text, monospace section labels in Snowball Blue `#0019FF`, Snowball Orange `#FF9000`
as a sparse accent. Brand colors follow SBC-INFRA-84; typography intentionally diverges
from it (website earns its own type).

## Deployment

Deployed via GitHub Pages from the `main` branch root. Pushing to `main` publishes to
https://snowball-consult.com (custom apex domain since 2026-08-17; www and http redirect there;
the `CNAME` file makes the custom domain work - never delete it). DNS lives at Strato; the full
runbook incl. the mail-safety rules is SBC-INFRA-128 in the `claude` repo.
