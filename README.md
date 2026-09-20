# snowball-website

Source for https://snowball-consult.com. Static single-page site, no build step: edit `index.html`, push to `main`, live.

## Status (V2, 2026-09-19)

One page, five sections, minimal header navigation:

1. **Hero** - "Precision GTM infrastructure for high-ACV markets." (the adopted LinkedIn banner
   line), a three-sentence lede, and the Claude Code-style status spinner (kept from V1, Esc or
   click interrupts it).
2. **Thesis** - the Decide / Build / Enable loop with the "What changes if we build this
   perfectly?" question and the 80/20 discernment paragraph. Copy is condensed from the
   2026-09-17 positioning elaboration and LinkedIn posts #031 / #032.
3. **Work** - four anonymized engagements (industry descriptor, what was built, sourced numbers
   only). No client names, no unsourced metrics. "Client names and references on request."
4. **Working together** - one or two clients, paid first phase, 3-6 months, upfront, no lock-in,
   leadership attention as precondition. No prices.
5. **About** - career (Kassel, Apple, backpacking, first-hire roles, Snowball Consult, Clay Club
   New York, Independent Consultant Meetup) plus a mono timeline. **Contact** - email + LinkedIn.

Sources and exclusions for the V2 copy are documented in the `claude` repo at
`snowball-service-offering/website/2026-09-19_v2-zero-shot-site-copy-sources-and-exclusions.md`.
V1 (spinner-only front page) and the 2026-08-17 dictated About copy remain in git history.

## Design

Bauhaus-leaning, restrained: FT paper `#FFF1E5`, Jost (Futura-like geometric sans, the only
third-party request) for all text, system monospace for labels and the spinner, Snowball Blue
`#0019FF` for structure (labels, numbers, links), Snowball Orange `#FF9000` as a sparse accent.
Three primary forms (circle / square / triangle) mark the three thesis elements and the hero.
Thick ink rules, thin paper rules, no cards, no shadows, no gradients. Single column under 860px.

## Deployment

GitHub Pages from the `main` branch root. Pushing to `main` publishes to
https://snowball-consult.com (apex custom domain; www and http redirect there; the `CNAME` file
makes the custom domain work - never delete it). DNS lives at Strato; the full runbook incl. the
mail-safety rules is SBC-INFRA-128 in the `claude` repo.
