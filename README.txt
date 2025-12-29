Dawn Galaxy Atlas (GitHub Pages, ONE QR code)

Put these 3 files in the ROOT of your GitHub Pages repo:
- index.html
- Book1.csv
- Planets_and_Stars_Esperanto.csv

QR Code:
- Enable GitHub Pages
- Your QR code points to: https://YOURNAME.github.io/REPO/
- You can update the CSVs any time. Keep filenames the same.

How updates work:
- index.html loads BOTH CSVs via fetch with a cache-busting query param (?v=Date.now()) so readers see your newest CSV immediately after you push commits.

File roles:
- Book1.csv: geometry + orbits (Type/Name/System Name/X/Y/Distance AU)
- Planets_and_Stars_Esperanto.csv: lore/details (Planet Name/Star Name/System Name/Species Name/etc.)

If Book1.csv is missing:
- The site will still render from the lore file using Planet Location / Star Location.

Notable Events:
- Any field matching “Notable Events” is hidden automatically.

Performance:
- Textured planet thumbnails are only shown for the selected planet and (when zoomed in) planets in the selected system, capped at 60.

