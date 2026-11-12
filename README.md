# Complications in Building a Nation: Five Delineations

A scrolling history walk about the German Colonial War Memorial that was never built on Berlin's Bersarinplatz.

## Repository layout

```
index.html
favicon.png            (tab icon)
apple-touch-icon.png   (icon when saved to a phone's home screen)
images/                (made by compress_images.py)
```

Do not commit `drive-images/` or `compress_images.py`'s originals; keep the full-size files in Google Drive.

## Preparing the pictures

1. Download your Google Drive picture folder and unzip it into `drive-images/` next to `index.html`. Subfolders are fine.
2. Make sure it also contains the new files: `background_light.png`, `background_dark.png`, `kaiser.jpg`, `bismarck.jpg`, `siegesallee.jpg` and `marchenbrunnen.jpg`.
3. Run `pip install pillow` once, then `python compress_images.py`.

The script finds every picture, gives it the name the website expects, shrinks it and saves it as `.webp` into `images/`. Missing or unreadable pictures are listed under "ERROR". Run it again after adding them: finished pictures are skipped. `python compress_images.py --force` redoes everything.

The full list of Drive names and website names is the `RENAME` table at the top of `compress_images.py`.

## Publishing on Vercel

Push the repository to GitHub, then import it in Vercel (framework: "Other", no build command). Every push updates the site.

## Editing

- **Captions, alt texts, hover texts and credits:** in `index.html`, search for `var SLOTS`. Each picture has `title` (caption), `alt` (read aloud by screen readers), `hover` (text near the cursor), `short` (credit under the picture) and `full` (entry in the image credits).
- **Footnotes:** search for `var NOTES`. They are numbered as in the essay.
- **Title flicker speed:** `FLICKER_PAUSE_MIN` and `FLICKER_PAUSE_MAX` near the top of the script.
- **Map flight:** open the page with `?mapdebug` added to the address, scroll to the map and click on Germany and on Kilimanjaro. Copy the two x/y pairs into `MAP_FROM` and `MAP_TO`. `MAP_FLIGHT_MS` sets how long the flight takes.
