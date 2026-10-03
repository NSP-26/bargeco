# Working Barge Co. site

One static page. Upload this folder as-is to any static host (Vercel, Netlify, Cloudflare Pages, S3).

- index.html has all markup, CSS and the small form script inline
- images/ has the two photos at 720px and 1200px wide, in WebP with JPG fallback, plus og.jpg for link previews

## Breakpoints

- 1100px and up: desktop layout
- 720 to 1099px: same layout with section labels above content, form in two columns
- under 900px: hero, data plate and drawing stack, use grid goes to two columns
- under 720px: phone layout (split nav bar, side-elevation-only drawing, single-column form)

## Form

Posts to FormSubmit (formsubmit.co), which emails each enquiry to hire@workingbargeco.com.
The first enquiry sends an activation email to that inbox. Click the link and it's live.
After that FormSubmit gives you a random alias. Swap it in for the address in the form
`action` and in `ENDPOINT` in the script so the address isn't in the page source.

Without JavaScript the form still posts and FormSubmit redirects back to
https://workingbargeco.com/?sent=1#contact. Change `_next` if the domain is different.

## Hero photo

There's a commented-out figure under the hero, with styles ready (.hero-photo).
Export it at 1200 and 2400px wide and uncomment.
