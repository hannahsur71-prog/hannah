# Isabelle Lee — Portfolio

A minimalist, professional portfolio site with photography and film kept as
separate categories, plus an About page. Plain HTML/CSS/JS — no build step,
works by opening `index.html` directly or hosting the folder as-is (GitHub
Pages, Netlify, Vercel, etc.).

## Structure

- `index.html` — home page with hero and links into Photography / Film
- `photography.html` — photo grid with a lightbox
- `film.html` — film project list (title, role, year, synopsis, link)
- `about.html` — bio + contact details
- `css/style.css` — all styling
- `js/script.js` — nav, scroll reveal, lightbox behavior
- `images/` — placeholder SVGs to swap for real photos/stills

## What still needs real content

The live Wix site (`isabellehaeunlee.wixsite.com/works`) could not be
reached from the build environment (network egress was blocked), so nothing
was copied from it. Everything here is original placeholder content to be
replaced:

1. **About text** — `about.html`, replace the two placeholder paragraphs
   with Isabelle's actual bio, plus the "Based In" / email / Instagram /
   availability details.
2. **Photos** — replace files in `images/photography/` with real images
   (keep the same filenames or update the `src`/`data-full` attributes in
   `photography.html`). Update captions in `data-caption`.
3. **Film projects** — replace `images/film/*.svg` with real stills or
   thumbnails, update titles, years, roles, synopses, and the `href` on each
   `.film-media` link to point to the actual video (YouTube/Vimeo).
4. **Home covers** — `images/home/photo-cover.svg` and `film-cover.svg`.
5. **Portrait** — `images/about/portrait.svg`.
6. **Contact links** — email address and Instagram handle in the footer and
   About page (currently placeholders).
7. **Name** — the display name "Isabelle Lee" is a placeholder based on the
   site's subdomain; update if her preferred display name differs.

## Local preview

Just open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`.
