# snowball-website

Source for www.snowball-consult.com. Static single-page site, no build step: edit `index.html`, push, live.

## Status

Front page (`index.html`) is a minimal widget: logo, tagline, and a Claude Code-style
status spinner cycling through 200 consulting/GTM-ops terms (Esc or click "interrupts" it),
plus a LinkedIn badge and an email-only footer (email@snowball-consult.com).
The About page (Andreas-dictated landing copy) is removed for the moment; the copy is
preserved in git history and in the `claude` repo at
`snowball-service-offering/website/2026-08-17_dictated-landing-copy-picking-the-right-problem.md`.
Purpose of the site: digital footprint plus a decent understanding of which type of problem
Snowball Consult solves. Planned later: blog and resources sections.

## Design

Deliberately minimal: centered column on FT paper `#FFF1E5`, Jost (Futura-like geometric
sans) for the tagline, monospace for the spinner line, Snowball Blue `#0019FF` for glyph
and links, Snowball Orange `#FF9000` as a sparse accent (rare terms, interrupt state).
Brand colors follow SBC-INFRA-84; typography intentionally diverges from it (website earns
its own type).

## Deployment

Deployed via GitHub Pages from the `main` branch root. Pushing to `main` publishes to
https://snowball-consult.com (custom apex domain since 2026-08-17; www and http redirect there;
the `CNAME` file makes the custom domain work - never delete it). DNS lives at Strato; the full
runbook incl. the mail-safety rules is SBC-INFRA-128 in the `claude` repo.
