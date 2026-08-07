# ERP logo files

Cards fall back to the vendor name in text when a file is missing, so the grid never looks broken.

## Present (9/11)
alert.png · current-rms.png · flex.png · insphire.png · point-of-rental.webp
rentman.svg · sirius.png · texada.webp · wynne.png

All have transparent backgrounds and render greyscale at 72% opacity, full colour on hover.

## Still needed (2)
| File | Vendor | Why it's missing |
|---|---|---|
| `mcs.svg` | MCS Rental Software | mcsrentalsoftware.com returns 403 to automated requests — download manually from the site |
| `intempo.svg` | InTempo | Their site renders the wordmark as CSS text, no image file exists — request from the vendor or set as text |

## Two to swap when you can
- **sirius.png** is the *Orion Software* corporate logo, not the *Sirius* product mark. Ask Gary for the Sirius brand file in the API thread — natural, low-stakes ask.
- **insphire.png** and **current-rms.png** are combined "X + Klipboard" lockups (both vendors were acquired by Klipboard). Standalone marks would look cleaner if you can find them.

## Specs
Max 30px tall / 132px wide, `object-fit: contain`. SVG preferred, PNG/WebP fine.
Use horizontal, transparent-background versions — anything with a baked-in white
background shows as a white box on the white card.
