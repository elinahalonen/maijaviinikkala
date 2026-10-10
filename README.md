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

## Status: private build

The site is built ahead of Maija's launch and written as an operating practice, in the present tense (see `docs/MAIJA_WEBSITE_COPY.md`, which is the source of truth for wording). Every page carries `<meta name="robots" content="noindex, nofollow">`; remove it at launch.

Pages: `index.html`, `palvelut.html`, `minusta.html`, `ennen-kayntia.html`, `yhteystiedot.html`, `tietosuoja.html`. Header and footer are repeated in each file, so a nav change means editing all six.

Bracketed items from the copy doc appear as small clay-coloured `.todo` labels. They are private build placeholders and must all be gone before launch: `grep -n 'class="todo"' *.html` lists them.

### Before launch

- Real portrait to replace `assets/images/concept-hero-placeholder*.jpg`; remove the `.concept-label` tag with it
- Location (paikkakunta), address and arrival instructions
- Phone, email, Y-tunnus
- Durations and prices for Hieronta and Urheiluhieronta; confirm both service names
- Exact professional title and qualifications for the "Koulutus ja osaaminen" section (or delete the section). Copy currently says "hieroja"; "koulutettu hieroja" is a protected title and needs Valvira (Terhikki) registration
- Booking route: once it exists, switch the "Ota yhteyttä" header and CTA buttons to "Varaa aika" (marked with comments)
- Booking and cancellation terms
- Privacy policy text (`tietosuoja.html`)
- Add the location to the page titles and descriptions, as in the copy doc's SEO section

### Images

The three images in `assets/images/` come from the moodboard. They appear to be AI-generated and are small (about 300 px wide), so they are displayed small and should be replaced with Maija's own photographs before launch. The hero currently uses the AI-generated concept portrait (`concept-hero-placeholder*.jpg`) for mockup purposes only. It is not a photograph of Maija, is tagged "Konseptikuva" on the page, and must be replaced before anything goes public.

Moodboard images left out on purpose: the candle-and-oil and metal bowl shots (closer to the rejected spa/incense direction) and the treatment room (it would read as a photo of her actual practice).

### Font note

The brand guide asks for Lato medium and semibold. The web distribution of Lato only has 400 and 700, so 700 is used for buttons and labels.
