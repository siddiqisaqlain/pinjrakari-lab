# Pinjrakari Lab

An interactive Islamic star pattern generator, inspired by Kashmiri pinjrakari lattice work.
Pick a tiling, turn the contact-angle dial, and export a real-scale drawing to CAD (DXF), SVG or PNG.

**Author:** Saqlain Siddiqi, B.Arch, IUST Awantipora, Kashmir
**Copyright:** © 2026 Saqlain Siddiqi

It is a static site: no build step, no server, no dependencies. Open `index.html` and it works.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole app (HTML, CSS, JavaScript) |
| `favicon.svg` | Browser tab icon (follows light/dark mode) |
| `apple-touch-icon.png` | Icon when saved to a phone home screen |
| `og-image.png` | Preview card shown when the link is shared (1200 × 630) |
| `.nojekyll` | Tells GitHub Pages to serve files as they are |

## Run locally

Double-click `index.html`, or from this folder run `python3 -m http.server` and open http://localhost:8000.

## Publish free on GitHub Pages

1. Create a GitHub account if you do not have one, then click **New repository**. Name it `pinjrakari-lab`, set it to **Public**.
2. Click **uploading an existing file**, drag in everything from this folder (including `.nojekyll`), and commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then **Save**.
4. After about a minute the site is live at `https://<your-username>.github.io/pinjrakari-lab/`.
5. Open `index.html` in the repository, click the pencil icon, and change both `og-image.png` values (the `og:image` and `twitter:image` lines) to the full address, for example
   `https://<your-username>.github.io/pinjrakari-lab/og-image.png`.
   Link previews on WhatsApp, LinkedIn and X need the full address.

## Alternative: Netlify (fastest)

Go to https://app.netlify.com/drop and drag this folder onto the page. You get a live link in seconds.
Then do step 5 above with your Netlify address.

## Later: your own website

- **Own domain:** buy one, then add it under GitHub **Settings → Pages → Custom domain** (or Netlify **Domain management**). HTTPS is automatic.
- **Part of a bigger site:** keep this folder as `/pinjrakari-lab/` inside the larger site, or link to it from a menu.
- **Update:** edit `index.html` and commit; the site refreshes by itself.

## Using the exports

- **DXF:** unzip the download. Units are millimetres, 1 drawing unit = 1 mm. Layers: `PATTERN`, `TILING`, `PANEL`, `TITLE`. Opens in AutoCAD, Rhino, Fusion, LibreCAD.
- **SVG:** millimetre sizes, opens in Illustrator, Inkscape, Figma, or a laser-cutter workflow.
- **PNG:** 2400 px, with a title strip.

## Credits

- Method: Hankin's polygons-in-contact, as described by Craig S. Kaplan.
- Reference paper: Lee, Kim and Jeon, on algorithmic control of Islamic star patterns, summarised at https://parametrichouse.com/the-islamic-star-pattern/
- This is a student project. Add a licence file (for example MIT, or "all rights reserved") before inviting others to reuse the code.
