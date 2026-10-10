# Maija Viinikkala: website

Static, Finnish-language one-page site. No framework, no build step.

- `index.html`: the page (header, hero, Palvelut, Minusta, Käytännössä, Ota yhteyttä, footer)
- `css/tokens.css`: brand colours, type and spacing (single source of truth, matches `docs/MAIJA_BRAND_GUIDELINES.md`)
- `css/site.css`: layout and components
- `assets/fonts/`: self-hosted Lora and Lato (SIL OFL 1.1). Self-hosted rather than loaded from Google, so visitors' IP addresses are not sent to a third party.
- `assets/images/`: provisional atmosphere images

## Preview

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

Open it over http rather than as a file, otherwise the browser blocks the preloaded fonts.

## Status: draft, not ready to publish

The page carries `<meta name="robots" content="noindex, nofollow">` and a visible draft banner. Remove both at launch.

Every detail not yet confirmed by Maija is shown on the page as a dashed `Vahvistetaan` marker (`.todo`). Nothing has been invented.

### Still needed from Maija

- A genuine portrait she has chosen (replaces `assets/images/concept-hero-placeholder*.jpg` in the hero; remove the `.concept-label` tag at the same time)
- Exact services, with description, who each is for, duration and price
- Professional title and qualification status, plus expected graduation date
- Background and working approach for `Minusta`
- Location and arrival instructions, opening hours, accessibility, cancellation terms, payment methods
- Contact details and booking route (only then add a "Varaa aika" button)
- Her own description of what happens on a first visit
- Business ID (Y-tunnus) for the footer
- Approval of the hero copy ("Hierontaa, johon on helppo tulla.")

### Images

The three images in `assets/images/` come from the moodboard. They appear to be AI-generated and are small (about 300 px wide), so they are displayed small and should be replaced with Maija's own photographs before launch. The hero currently uses the AI-generated concept portrait (`concept-hero-placeholder*.jpg`) for mockup purposes only. It is not a photograph of Maija, is tagged "Konseptikuva" on the page, and must be replaced before anything goes public.

Moodboard images left out on purpose: the candle-and-oil and metal bowl shots (closer to the rejected spa/incense direction) and the treatment room (it would read as a photo of her actual practice).

### Font note

The brand guide asks for Lato medium and semibold. The web distribution of Lato only has 400 and 700, so 700 is used for buttons and labels.
