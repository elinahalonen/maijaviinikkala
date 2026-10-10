# Claude Code handoff | Maija Viinikkala website

You are implementing a Finnish-language website for **Maija Viinikkala**, a professional massage practitioner launching her own practice **after completing her training**. Read `MAIJA_BRAND_GUIDELINES.md` for visual rules and `MAIJA_WEBSITE_COPY.md` for the proposed Finnish copy. Treat the copy file as the source of truth for page wording, subject to Maija’s final approval. First inspect the existing repo, identify its framework and assets, and propose the smallest effective changes. Preserve any existing content and functionality that are correct.

## Critical timing and copy rule

**Build privately now, launch after qualification.** The website must read as a fully operating, professional massage practice from its first public day. Write copy **in the present tense**, e.g. "Tarjoan yksilöllistä hierontaa", "Tutustu palveluihin", "Varaa aika". Do **not** say or imply Maija is still studying, waiting to graduate, not yet qualified, or about to start offering massage. The timing of the build is an internal project detail.

Before publishing, verify that her training is complete and confirm the exact legally appropriate Finnish professional title, services, and specialisms. Do not invent a credential; if the title is pending confirmation, use "Maija Viinikkala | Hierontaa ja hyvinvointia" and neutral service descriptions in the private build. She expects sports massage to be part of the offer; confirm its wording and availability for launch. Pregnancy massage and breastfeeding advice must not appear as currently bookable unless she verifies that she is qualified and offers them at launch.

## Direction

Build a **warm, bright, refined, editorial** identity that looks like a credible personal massage practice, not a mystical retreat, beauty salon, corporate clinic or generic wellness template. Maija chose the light, raspberry-led option with subtle green. She wants green present but not dominant. She rejected a more incense-like aesthetic and does not want her personally meaningful triple-moon symbol used on the website.

## Brand tokens

```css
:root {
  --brand-raspberry: #8D3558;
  --brand-ivory: #F8F5F0;
  --brand-gold: #CFA251;
  --brand-green: #5A6B56;
  --brand-pale-clay: #E9D4C9;
  --brand-plum: #352A35;
  --brand-white: #FFFFFF;

  --color-page: var(--brand-ivory);
  --color-text: var(--brand-plum);
  --color-heading: var(--brand-raspberry);
  --color-primary-action: var(--brand-raspberry);
  --color-secondary-panel: var(--brand-pale-clay);
}
```

Use **Lora** for large headings and **Lato** for body/UI, with fallback fonts. Place all design tokens in a central stylesheet or theme configuration.

## Website priorities

1. A simple header with name, clear service descriptor and navigation.
2. A light hero with a **genuine, Maija-approved portrait** for publication (concept image acceptable only in the private draft) and a clear, confident statement of the services offered at launch.
3. Visible services presented as active professional services, with their descriptions and booking/contact routes (verify before launch).
4. A concise `Minusta` section introducing Maija as a professional, with only verified qualifications and facts.
5. Practical information visitors need before booking.
6. Strong mobile layout, readable typography, clean metadata, sensible page structure, accessible keyboard navigation and contrast.

Do not use a mockup's AI-generated portrait as if it were a genuine photograph of Maija. If approved photos are not in the repository, use an explicitly labelled placeholder, not a fabricated personal portrait.

## Important restrictions

- Do not invent prices, location, contact details, operating hours, qualifications, certifications, appointment availability or testimonials.
- Pregnancy massage and breastfeeding advice are potential future directions. Do not present either as bookable unless Maija confirms she is qualified and will offer them at launch.
- Avoid lotus icons, triple moons, crystals, incense, glitter textures and overdecorated botanical motifs.
- Avoid a large dark-green hero, dark forest atmosphere and large blocks of orange/gold. Green is a selective secondary colour. Gold is for fine accents only; do not put gold body text on ivory.
- Use real, natural-light photographs where licensed and approved. The design should communicate freshness, warmth, professional confidence and easy access to information.
- Keep Finnish copy natural and concrete. Avoid unverified therapeutic or medical promises.

## Public-facing Finnish copy

Use **`MAIJA_WEBSITE_COPY.md`** for the complete launch-time homepage, services, about, FAQ, contact and SEO wording. The draft intentionally reads as an active, qualified practitioner’s site. Use natural Finnish and preserve the approved professional, warm tone. Do not include statements about education still being in progress or the site being prepared early. Replace bracketed internal placeholders before the site goes live. Adjust the exact service names and business facts using information Maija supplies.

## Social media compatibility

Build an optional `/brand` or internal reference page only if requested, showing typography, colours, buttons, card styles and four reusable social composition examples described in the brand guide. The same token values should be easy to reuse in Canva or social templates, but the website itself does not need social-post creation functionality.

## Working method

1. Show the proposed file changes and confirm what assets and business details are missing.
2. Implement the minimal viable site and check it in mobile and desktop layouts.
3. Run the repo's build/lint/test commands where available.
4. Summarise what was changed, any private-build placeholders, and what Maija must approve before launch. Do not expose the pre-graduation build status to public visitors.
