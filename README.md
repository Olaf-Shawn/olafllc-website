# Olaf LLC — Website

Static marketing site for **Olaf LLC** — an operator-led firm: AI advisory &
development, real estate lending, a real estate fund / distressed assets, and
capital & partner introductions.

## Stack

Plain HTML/CSS/JS. **No build step, no framework, no bundler.** Each page is
self-contained (CSS in a `<style>` block in its own `<head>`). Open any
`.html` directly in a browser, or deploy the folder as a static site.

## Brand

- **Palette:** gold (`#B8922E`) on warm cream (`#F7F4ED`), with deep warm-ink
  (`#1A1611`) dark sections. Distinct from the GCM brand.
- **Type:** Cinzel (small-caps accents, matches the logo), Playfair Display
  (headings), Inter (body) — loaded via Google Fonts.
- **Logo:** `assets/olaf-logo-gold.png` (gold triquetra wordmark, for light
  sections) and `assets/logo-white-cropped.png` (reversed, for dark sections).

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Home — umbrella story + 4 service sections (AI / Lending / Fund / Capital), about, process, contact. |
| `privacy.html` | Privacy Policy. |

Planned next: dedicated `ai.html`, `lending.html`, `fund.html`, `capital.html`
landing pages (each targeting its own search intent) + an `insights/` blog.

## TODO before launch

- [ ] Replace `assets/olaf-logo-gold.png` with a higher-res / SVG export
      (current is 394x259 — soft on retina).
- [ ] Wire the contact form to a real backend (Formspree / Power Automate /
      etc.) — see the `FORM_ENDPOINT` note in `index.html`. It confirms
      locally but does not transmit yet.
- [ ] Confirm a contact email address to publish.
- [ ] Legal review of `privacy.html` and the mortgage compliance footer.
- [ ] Point `olafllc.com` DNS at the static host once ready (currently
      WordPress on Bluehost).

## Reference

`reference/` holds an archived copy of the previous WordPress site's pages
(Home + Privacy) for content reference. Not part of the deployed site.

## Deploy

Any static host (Vercel, Netlify, Cloudflare Pages, GitHub Pages). No server
or database required.
