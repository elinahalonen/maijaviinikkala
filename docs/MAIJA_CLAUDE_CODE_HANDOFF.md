# Claude Code handoff | Maija Viinikkala website

You are implementing a Finnish-language website for **Maija Viinikkala**, a massage practitioner establishing her own practice. Read `MAIJA_BRAND_GUIDELINES.md` as the visual/content source of truth. First inspect the existing repo, identify its framework and assets, and propose the smallest effective changes. Preserve any existing content and functionality that are correct.

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
2. A light hero with a **genuine, Maija-approved portrait** and an immediately understandable statement of the current service offering.
3. Visible services with their descriptions and booking/contact routes.
4. A concise `Minusta` section with only confirmed facts.
5. Practical information visitors need before booking.
6. Strong mobile layout, readable typography, clean metadata, sensible page structure, accessible keyboard navigation and contrast.

Do not use a mockup's AI-generated portrait as if it were a genuine photograph of Maija. If approved photos are not in the repository, use an explicitly labelled placeholder, not a fabricated personal portrait.

## Important restrictions

- Do not invent prices, location, contact details, operating hours, qualifications, certifications, appointment availability or testimonials.
- Pregnancy massage and breastfeeding advice may be future directions, not current services. Ask for verification before displaying either as bookable or qualified services.
- Avoid lotus icons, triple moons, crystals, incense, glitter textures and overdecorated botanical motifs.
- Avoid a large dark-green hero, dark forest atmosphere and large blocks of orange/gold. Green is a selective secondary colour. Gold is for fine accents only; do not put gold body text on ivory.
- Use real, natural-light photographs where licensed and approved. The design should communicate freshness, warmth, professional confidence and easy access to information.
- Keep Finnish copy natural and concrete. Avoid unverified therapeutic or medical promises.

## Social media compatibility

Build an optional `/brand` or internal reference page only if requested, showing typography, colours, buttons, card styles and four reusable social composition examples described in the brand guide. The same token values should be easy to reuse in Canva or social templates, but the website itself does not need social-post creation functionality.

## Working method

1. Show the proposed file changes and confirm what assets and business details are missing.
2. Implement the minimal viable site and check it in mobile and desktop layouts.
3. Run the repo's build/lint/test commands where available.
4. Summarise what was changed, anything still placeholder, and what Maija must approve before launch.
