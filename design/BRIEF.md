# Working Barge Co. — build brief

Static one-page marketing site for a 12m work barge hire business in NSW. Two reference layouts are in this folder, exported from the design canvas. They are plain HTML with inline styles, meant as a visual reference, not as production code. Build one responsive page from them.

## Files

- `desktop.html` — full desktop layout, fixed 1440px wide
- `mobile.html` — full phone layout, fixed 390px wide
- `brand-sheet.html` — marks, colours, type scale, UI elements, design rules
- `desktop.png`, `mobile.png`, `brand-sheet.png` — the same three, rendered
- `images/` — the two real photos the layouts use, referenced as `images/…` from both HTML files

Both layouts are the same content in the same order. Treat desktop as the wide breakpoint and mobile as the narrow one, and pick sensible behaviour in between.

## Brand

Typeface: IBM Plex Mono only, weights 400, 500 and 600, loaded from Google Fonts.

Colours:

- Sand `#E8E2D5` — page background
- Stone `#DDD6C7` — panels and the contact band
- Charcoal `#1D1D1B` — text, 1px rules, buttons
- Graphite `#5A574F` — labels and captions, plus the use section, photo placeholders and footer as a background with sand text
- Signal `#B8431F` — hover state only

Rules: 1px charcoal rules for all structure, square corners, no shadows, no gradients, no animation, no icons unless a label cannot do the job. Sections are numbered like a manual (01 / HIRE, FIG. 2, DWG. WB-01). Photos are documentary, not glossy.

## Page order

1. Meta strip and nav (HIRE / SPECS / TRANSPORT / CONTACT, anchor links)
2. Hero: "12M WORK BARGE HIRE", location line, hire-type list, enquiry button
3. 01 / HIRE intro
4. 02 / SPECS: data plate table and the general arrangement drawing, inline SVG
5. 03 / USE: six numbered cells on a graphite background
6. 04 / TRANSPORT: text and two photo frames
7. 05 / CONTACT: "NEED A BARGE?" and the hire enquiry form
8. Footer

## To finish

- The transport section has the two real photos in it, captioned FIG. 1 and FIG. 2. They are cropped with `object-fit: cover`, so keep that behaviour and serve properly sized versions.
- Neither layout has a hero photo. There is an empty slot under the hero on both if one gets added.
- The form is markup only. It needs a backend or a form service, sending to hire@workingbargeco.com.
- Contact is email only: hire@workingbargeco.com. No phone, no address, no ABN yet.
- Vessel: unit WB-01, 12m long, 8m beam, 1m depth, dry or crewed hire, Sydney Harbour and Pittwater.
- The drawing is marked indicative and not to scale. Keep that note if the dimensions stay approximate.
