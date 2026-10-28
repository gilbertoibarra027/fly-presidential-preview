# Fly Presidential: concept preview sources and licenses

This is a concept preview by GEIT Marketing. It uses placeholder copy and is not affiliated content.
No text or images were taken from flypresidential.com.

## Reference photos (labelled "Reference photo" on the page)

These four photos were **provided by Gilberto (reference, likely Pexels)**.
- Originals are stored in `src/user/`.
- The license and photographer have not been confirmed. Check each one on Pexels, or replace it, before any public launch.

| Page file | Original file | Content | Used in |
|---|---|---|---|
| hero-ramp.jpg | 01M62BAF2NK0J6GE9BCNMN5RWK.jpg | Jets on a ramp under a blue sky | Hero opening frame |
| charter.jpg | 01M62BAP5Q34YBVGT41RBTTXPK.jpg | Jet at sunset with its stairs down | Charter |
| boarding.jpg | 01M62BAQPQ1R12BR6JAZYEFZAA.jpg | Passenger boarding a jet | Experience (inset) |
| hangar.jpg | 01M62BAH7GR38DM1AGC52CX481.jpg | Engine and tail in a hangar | Fleet |

The only processing was resizing, cropping and JPEG re-encoding (`build/assets.py`).

## AI concept images (labelled "AI concept" on the page)

Gilberto approved these AI-generated images for the concept. Originals are stored in `src/ai/`.

**A: white jet climbing toward a cloud bank** (A_jet_climb.jpg, 1280×720). `build/cut_jet.py` split it into three files:
- `jet.webp`: a cutout of the jet with transparency, animated in the hero.
- `sky.jpg`: a sky plate with the jet removed by inpainting. It is the hero background and also the Destinations band.
- `clouds.webp`: the cloud bank with transparency. It is the rising parallax cloud layers in the hero; the second layer is mirrored.

**B: near-white cloud interior** (B_cloud.jpg) becomes `cloud-white.jpg`, the hero's final white-out layer.

**C: luxury cabin interior** (C_cabin.jpg) becomes `cabin.jpg`, used in Experience.

## Stock

Pexels was tried directly, but pexels.com and videos.pexels.com returned HTTP 403, so no stock files were downloaded. No other stock was used.

## Fonts

Cormorant Garamond and Inter are loaded from the Google Fonts CDN under the SIL Open Font License 1.1.

## Code

All HTML, CSS and JS was written for this mockup. It has no third-party libraries.

## Content and claims

- All copy is placeholder. Homepage lines were supplied by Rex.
- Aircraft categories (Light, Midsize, Heavy) and destinations are labelled as examples.
- There are no tail numbers, aircraft specs, safety ratings, certifications (no ARGUS or Wyvern claims) or prices.
- The quote form is mockup-only: it submits nowhere.
- The page is `noindex,nofollow`, and robots.txt disallows everything.
