
# The Cyber Times

A newspaper-style crime report that turns a presentation topic into an interactive web page: **a CEO impersonation scam carried out through a fake Facebook profile and mobile banking (MFS) transfers in Bangladesh.**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Open%20the%20Site-BA0000?style=for-the-badge&logo=render&logoColor=white)](https://cyber-times-onrender-com.onrender.com/)

**Live site:** https://cyber-times-onrender-com.onrender.com/
**Status:** Educational case study

---

## The case

Fahim downloads public LinkedIn photos and details belonging to CEO Farhan Ahmed and opens a fake Facebook account using his full name and the company's branding. He sends urgent messages to three department managers, claims a medical emergency while travelling abroad, and persuades them to transfer BDT 2 Lakhs by mobile banking. The fraud is discovered when the real CEO returns. The company reports the profile, cyber police trace the mobile wallet to Fahim's real national ID registration, and he is arrested and charged.

## What is on the page

- **Masthead and utility bar:** blackletter title, weather, issue number, edition, and a section nav with an active state.
- **Hero:** a split layout with a red kicker, headline, deck, byline and pull quote, beside a collage illustration with an "Evidential Exhibit" stamp.
- **Story:** a two-column justified article with a drop cap, then a "Harvesting what was already public" feature.
- **Following the Money:** an illustrated MFS audit trail from the three transfers to the NID-linked wallet and its freeze.
- **The Charges:** seven charge boxes, each with the act, section, offence and description, plus a Summary of Charges table.
- **The Punishment:** a boxed list in italic type.
- **Sidebar:** a Case File card, a timeline numbered 01 to 06, an "Also in Business" story, and a Corporate Advisory card.
- **Corporate Advisory:** six safeguards with `CRITICAL`, `MANDATORY`, `URGENT` and `HIGH` priority badges, a short explanation under each, tick boxes and a live progress counter.
- **Controls:** a floating dark/light toggle and a Mobile/Desktop view simulator (390px preview).

## Legal references used

| Act / Code | Section | Offence |
|---|---|---|
| Cyber Security Act 2023 | 24 | Identity theft and digital impersonation |
| Cyber Security Act 2023 | 23 | Digital / electronic fraud |
| Cyber Security Act 2023 | 26 | Unauthorized collection / use of identity details |
| Penal Code 1860 | 416 & 419 | Cheating by personation |
| Penal Code 1860 | 420 | Cheating and inducing delivery of property |
| Penal Code 1860 | 468 & 471 | Forgery for the purpose of cheating |
| Money Laundering Prevention Act 2012 / MFS rules | n/a | Receiving fraud proceeds in an NID-linked wallet |

> **Disclaimer:** Section numbers were supplied by the project author and are not legal advice. Verify them against the official text of each law before relying on them. The case number, timestamps, account age and the "Central Bank" side story are **illustrative placeholders**.

## Design

- **Concept:** a modern broadsheet crime report with a collage feel: red slab accents, halftone illustration, a faint paper grain, hairline rules and double rules.
- **Palette:** newsprint `#F4F1EA`, ink `#111111`, slate `#444444`, crimson `#BA0000`. The dark theme uses `#15120E`, `#EFE9DA` and `#FF4A4A`.
- **Typography:**
  - UnifrakturMaguntia: masthead
  - Playfair Display (900): headlines
  - Source Serif 4: body text
  - Cormorant Garamond (italic): decks, quotes and punishments
  - JetBrains Mono: labels, legal codes and IDs
- **Layout:** CSS grid with container queries, so the mobile preview toggle and real phones use the same layout rules.
- **Accessibility:** visible keyboard focus, real buttons and checkboxes, light and dark themes, and reduced-motion support.
- **Components:** `.c-kicker`, `.c-case-row`, `.c-charge-badge` and the figure and advisory cards.

## Project structure

```
cyber-times/
├── index.html    # the whole site: HTML, CSS, JS and embedded images
├── render.yaml   # Render static-site config
├── README.md
└── .gitignore
```

No build step, no dependencies. Fonts load from Google Fonts.

## Run locally

Open `index.html` in any modern browser.

## Deploy on Render

1. Push this repo to GitHub.
2. In Render, choose **New → Static Site** and connect the repo.
3. Leave **Build Command** empty and set **Publish Directory** to `.`
4. Create the site. Every push to `main` redeploys automatically.

## Design prompts

The look was developed iteratively and the prompts can be reused in Figma, Dribbble shots or Lovable. The key brief:

> Redesign "The Cyber Times" as a high-density editorial front page in the style of an investigative newspaper issue. Blackletter masthead, huge red serif headline, two-column justified story with a drop cap, evidence collage hero, a charges grid, a punishment box in italic type, a case file and timeline sidebar, and a corporate advisory card with priority badges. Newsprint, ink and crimson palette. Responsive, with dark mode.

## Credits

- Illustrations: _add the source and licence for the three images used in the hero, "Har
