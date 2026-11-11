# GSK Plumbing Solutions: location page writer notes

**Layout name:** GSK suburb service landing page (the Next.js "ServiceLandingPage" template on the live site)
**Source pages (approved, built by delivery):**
- https://gskplumbingsolutions.com.au/blocked-drain-plumber-randwick
- https://gskplumbingsolutions.com.au/blocked-drain-plumber-coogee

**Use for:** suburb location pages, e.g. "Blocked Drain Plumber in Bondi Junction", "Plumber Marrickville", "Blocked Drains Burwood".
**Files:** `skeleton.html` (fill every `{{...}}` slot and delete the slot comments), `sample.html` (Bondi Junction worked example), `page_css.css`, `page_header.html`, `page_footer.html`.

## Rules
- Exactly one `<h1>`. The hero `<section>` keeps `class="pg-hero gs gs-hero"`. Every top-level block keeps the `gs` class.
- No inline `style` attributes. Only the classes already used in the skeleton.
- Australian English. No em or en dashes (use commas or full stops). No Oxford comma. Hyphenated compounds the live site uses are fine (high-pressure, drain-cleaning, on-site).
- Never invent facts. Only reuse the facts listed under "Facts on the live pages". No prices, years in business, team names, awards or guarantees that are not listed.
- Do not make claims about the suburb you cannot stand behind (no council names, street names, housing age figures). Neutral property types (houses, apartments, units, shops, commercial premises) are fine.
- Headings are one colour on this site. **No two-tone spans** (unlike TLC). Section H2s carry `class="gs-acc"` (blue gradient underline bar), except the two dark CTA bands (`gs-cta`), whose H2 has no class.
- Live casing: Title Case for section H2s; sentence case for the two CTA band H2s ("Blocked drain emergency? We're ready 24/7", "Need a blocked drain plumber in Randwick?").

## Sections in order (word budgets from the live pages)
| # | Section (class) | Variable? | What to write |
|---|---|---|---|
| 1 | Hero `section.pg-hero.gs-hero` | Partly | Eyebrow 3 to 5 words, uppercase (live: "FAST &amp; RELIABLE DRAIN SERVICES"). H1 5 to 9 words with the service keyword and suburb (live: "Expert Blocked Drain Plumber in Randwick", "Professional Blocked Drain Clearing in Coogee"). Lead 15 to 22 words, one sentence. The three ticks are **fixed**. The form card is **fixed** except the Service required value. |
| 1b | Mobile hero image `img.gs-mimg` | Image only | Same photo as the hero background, with real alt text "GSK Plumbing Solutions [service] in [Suburb]". Shown on mobile only, as on the live site. |
| 2 | Trust strip `section.gs-trust` | **Fixed** | Five badges, verbatim. |
| 3 | Intro split | Yes | Eyebrow (live: "CLEAR SOLUTIONS"). H2 6 to 10 words. P1 45 to 60 words (the problem, then we provide [service] across Sydney, including [Suburb], inspect, find the cause, recommend the method). P2 30 to 50 words (methods, communication, workmanship, testing). Four ticks of 3 to 6 words. Buttons fixed. Framed photo on the right, alt "GSK Plumbing Solutions [service] services in [Suburb]". |
| 4 | Services grid `gs-soft` | Yes | H2 "Our [Service] Services in [Suburb]". 6 to 7 cards: icon + H3 (2 to 5 words) + P (13 to 18 words, "We ..." voice). Name the suburb in two or three cards, not all. |
| 5 | Emergency band `gs-cta` (mirrored water background) | Partly | H2 5 to 8 words (live: "Blocked drain emergency? We're ready 24/7"). P 22 to 30 words ending "...anywhere in [Suburb]." Buttons and the three mini cards are fixed. |
| 6 | Why choose | Nearly fixed | Team photo and eyebrow fixed. H2 "Why [Suburb] Property Owners Choose Our Plumbers". Only the first item's sentence changes (10 to 16 words: local team, the suburb and Sydney). The live first sentence reads awkwardly ("experienced with blocked drain plumbers in randwick"), so write it cleanly. The other five items are verbatim. |
| 7 | Process `gs-dark` | **Fixed** | Four steps, verbatim. |
| 8 | Service areas `gs-soft` | **Fixed** | 32 suburbs and the "Don't see your suburb?" box, verbatim. Do not add the page's suburb to this list. |
| 9 | FAQ | Yes | H2 "Frequently Asked Questions about [Service]" (live says "about Block Drains", a typo; write "Blocked Drains"). Five Q&amp;As: 3 in the left column, 2 in the right, the first one `open`. Questions 6 to 14 words, answers 25 to 45 words. Live mix: signs of the problem; do you service [Suburb] (or apartments in [Suburb]); a method question (jetting, CCTV); emergency help in [Suburb]; when to call or what to do while waiting. Start yes or no answers with "Yes." |
| 10 | Final CTA `gs-cta` | Partly | H2 "Need a [service] in [Suburb]?". Three ticks (a speed point, a method point, "Licensed [Suburb] plumbers"). Call button and the "SEND US A MESSAGE" form fixed except the Service required value. |

**Total:** 750 to 900 words including fixed copy and form labels (Randwick shows about 690 visible words plus about 130 in the collapsed FAQ answers; the Bondi Junction sample is about 880). The variable copy you write is about 450 to 550 words.

**Tone on the live pages:** plain and practical, "we" voice, short declarative sentences, no hype, no exclamation marks, no questions in body copy. Themes: inspect, identify the cause, choose the right method, clear communication, tidy work, test before leaving.

## Fixed copy (already in the skeleton, copy verbatim)
- Hero ticks: Same Day Service / Upfront, Fixed Pricing / Licensed &amp; Insured Plumbers
- Hero form: "Get Fast Help Now", "Request a call back or book online.", fields Full name *, Phone number *, Suburb *, Service required *, Message (optional), button "Get Help Now", note "We'll call within 10 minutes". Final form: eyebrow "SEND US A MESSAGE", same fields, button "Send Message".
- Service required options on the live form: Blocked drain, Blocked toilet, Hot water, Gas fitting, Burst pipe or leak, Leaking tap or toilet, Emergency plumbing, Commercial plumbing, General plumbing, Other. Pick the one matching the page (Blocked drain for blocked drain pages, General plumbing for "Plumber [Suburb]").
- Trust strip: 5 stars / 200+ 5 star reviews; On-site fast / Prepared Sydney plumbers; Licensed &amp; insured / NSW contractor licence 346665C; Sydney local / All of Sydney; 24/7 emergency / 24/7 emergency plumbing
- Emergency minis: 24/7 emergency service / On-site fast / Upfront prices
- Why items 2 to 6, the process steps, the service area list and the "Don't see your suburb?" box
- Buttons: "Call 1300 241 326" (tel:1300241326) and "Get a Quote" (links to /contact in the mockup; on the live site it opens a quote pop-up)

## Images
- Hero (used twice, desktop background and mobile image) and the intro image are variable. Use the client's photo library, following the TLC hub pattern: `https://update.readytorank.com.au/gsk-plumbing-hub/img/pages/<mon>/<slug>-hero.jpg`, `-1.jpg`. If no new photo exists, the live site's own photos may be reused: `https://gskplumbingsolutions.com.au/images/blocked-toilet.jpg`, `blocked-toilet-2.jpg`, `blocked-drains-2.jpg` (Randwick and Coogee use these). Landscape, 1024x683 ratio.
- The team photo `local-team-2.jpg` and the water texture `section-background.png` are fixed.
- Alt text pattern: "GSK Plumbing Solutions [service] in [Suburb]" (hero), "GSK Plumbing Solutions [service] services in [Suburb]" (intro).

## Service card icons (paste inside `<i class="gs-ico">`)
- **waves**: `<svg viewBox="0 0 24 24"><path d="M2 6c.6.5 1.2 1 2.5 1C7 7 7 5 9.5 5c2.6 0 2.4 2 5 2 2.5 0 2.5-2 5-2 1.3 0 1.9.5 2.5 1M2 12c.6.5 1.2 1 2.5 1 2.5 0 2.5-2 5-2 2.6 0 2.4 2 5 2 2.5 0 2.5-2 5-2 1.3 0 1.9.5 2.5 1M2 18c.6.5 1.2 1 2.5 1 2.5 0 2.5-2 5-2 2.6 0 2.4 2 5 2 2.5 0 2.5-2 5-2 1.3 0 1.9.5 2.5 1"/></svg>`
- **toilet**: `<svg viewBox="0 0 24 24"><path d="M7 12h13a1 1 0 0 1 1 1 5 5 0 0 1-5 5h-.6a1 1 0 0 0-.95 1.32L15 22H9l1-3.5A6 6 0 0 1 4 12V4a2 2 0 0 1 2-2h2a2 2 0 0 1 2 2v8"/></svg>`
- **rain**: `<svg viewBox="0 0 24 24"><path d="M4 14.9A7 7 0 1 1 15.7 8h1.8a4.5 4.5 0 0 1 2.5 8.2M16 14v6M8 14v6M12 16v6"/></svg>`
- **search**: `<svg viewBox="0 0 24 24"><circle cx="11" cy="11" r="8"/><path d="m21 21-4.3-4.3"/></svg>`
- **droplets**: `<svg viewBox="0 0 24 24"><path d="M7 16.3c2.2 0 4-1.83 4-4.05 0-1.16-.57-2.26-1.71-3.19S7.29 6.75 7 5.3c-.29 1.45-1.14 2.84-2.29 3.76S3 11.1 3 12.25c0 2.22 1.8 4.05 4 4.05zM12.56 6.6A11 11 0 0 0 14 3c.5 2.5 2 4.9 4 6.5s3 3.5 3 5.5a7 7 0 0 1-11.91 4.97"/></svg>`
- **wrench**: `<svg viewBox="0 0 24 24"><path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94z"/></svg>`
- **clock**: `<svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><path d="M12 6v6l4 2"/></svg>`
- **shield**: `<svg viewBox="0 0 24 24"><path d="M20 13c0 5-3.5 7.5-7.66 8.95a1 1 0 0 1-.67-.01C7.5 20.5 4 18 4 13V6a1 1 0 0 1 1-1c2 0 4.5-1.2 6.24-2.72a1.17 1.17 0 0 1 1.52 0C14.51 3.81 17 5 19 5a1 1 0 0 1 1 1z"/></svg>`
- **truck**: `<svg viewBox="0 0 24 24"><path d="M14 18V6a2 2 0 0 0-2-2H4a2 2 0 0 0-2 2v11a1 1 0 0 0 1 1h2M15 18H9M19 18h2a1 1 0 0 0 1-1v-3.65a1 1 0 0 0-.22-.62l-3.48-4.35A1 1 0 0 0 17.52 8H14"/><circle cx="17" cy="18" r="2"/><circle cx="7" cy="18" r="2"/></svg>`
- **sparkles**: `<svg viewBox="0 0 24 24"><path d="M12 3l1.9 5.8L20 11l-6.1 2.2L12 19l-1.9-5.8L4 11l6.1-2.2z"/></svg>`

Live mapping on drain pages: Clearing = waves, Toilet = toilet, Sewer and stormwater = rain, CCTV = search, Jetting = droplets, Tree roots = wrench, Emergency = clock. For general plumbing pages pick from wrench, droplets, shield, truck, sparkles and clock.

## Internal links
- The live location pages have **no in-body text links**, only the phone (tel:1300241326) and Get a Quote buttons. Keep it that way; do not add links inside paragraphs.
- The header and footer files carry the site navigation. Live service URLs for reference: /plumbing-services, /emergency-plumber-sydney, /blocked-drains, /blocked-toilets, /hot-water-services, /gas-fitting, /leaking-taps, /burst-pipes, /commercial-plumbing, /service-areas, /contact, /about-us, /gallery, /blog.
- Existing location pages (do not duplicate): blocked-drain-plumber-hurstville, -st-george, -southern-sydney, -kensington, -kogarah, -randwick, -maroubra, -paddington, -coogee, -rockdale. Live URL pattern: `/blocked-drain-plumber-[suburb]`.
- Body copy uses "drain cleaning services in Sydney" and "blocked drain repair in Sydney" as plain text (likely target terms). Reuse naturally, unlinked.

## Facts on the live pages (the only facts you may use)
| Fact (verbatim) | Where it appears |
|---|---|
| 1300 241 326 (tel:1300241326) | Header, body buttons and footer on both source URLs |
| info@gskplumbingsolutions.com.au | Footer, both source URLs |
| NSW contractor licence 346665C | Trust strip and footer, both source URLs |
| Work completed by qualified plumbers under NSW licence 346665C. | Why section, both source URLs |
| ABN 26 638 872 036 | Footer, both source URLs |
| 5 stars / 200+ 5 star reviews | Trust strip, both source URLs |
| 24/7 Emergency Service; 24/7 emergency plumbing; 24/7 emergency availability | Header bar, trust strip, footer |
| Same-Day Service; Same Day Service; Same day service available | Header bar, hero ticks, final CTA |
| Licensed &amp; Insured Plumbers | Header bar, hero ticks |
| Upfront Pricing &amp; Sydney-Wide Coverage; Upfront, Fixed Pricing; Upfront prices | Header bar, hero ticks, emergency minis |
| We'll call within 10 minutes | Hero form note, both source URLs |
| CCTV inspection and jetting; high-pressure water jetting; CCTV equipment | Services and final CTA, both source URLs |
| Prepared vehicles and professional tools for efficient diagnosis and repairs. | Why section |
| 100% satisfaction | Why section |
| GSK Plumbing Solutions provides residential, commercial and 24/7 emergency plumbing across Sydney. Our licensed team handles blocked drains, hot water, gas fitting, leaks, burst pipes and general plumbing with clear communication and upfront pricing. | Footer blurb |
| Instagram: instagram.com/gskplumbingsolutions | Footer |

Not stated on these pages: years in business, owner or plumber names, prices, call-out fees, warranties, a street address. Do not add them.

## Avoid
- Em or en dashes, Oxford commas, American spelling.
- Two-tone headings or `<span>` inside headings.
- The suburb in every sentence. Aim for it in the H1, lead, intro H2, P1, services H2, 2 to 3 cards, emergency P, why H2, 2 FAQs and the final H2.
- Changing fixed sections, adding sections or adding a sidebar (this layout has none).
- Reusing the Randwick or Coogee wording word for word; write each variable block fresh for the new suburb.
