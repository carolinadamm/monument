# Complications in Building a Nation: Five Female Voices

A scrolling history walk about the German Colonial War Memorial that was never built on Berlin's Bersarinplatz.

## Repository layout

```
index.html
images/
  char-jagodja-1891.png
  ...
```

Put every picture into a folder called `images` next to `index.html`, renamed as listed below. The ending (.jpg, .jpeg or .png) doesn't have to match: the page also tries the other endings. A picture that is missing shows as a labelled box with the expected file name, so you can spot gaps quickly.

To publish: Settings → Pages → Deploy from branch → `main` / root. The site appears at `https://<your-name>.github.io/<repository>/`.

## Rename your Drive files like this

| Drive file | Rename to |
|---|---|
| Jagodja_1895.PNG | char-jagodja-1891.png |
| Rosa Luxemburg.PNG | char-rosa-luxemburg.png |
| Hedwig Heyl.PNG | char-hedwig-heyl.png |
| Agnes von Boemcken.PNG | char-agnes-von-boemcken.png |
| Jagodja_2026.PNG | char-jagodja-2026.png |
| First pic - Bersarinplatz as if elephant was there today.png | plaza-with-monument.png |
| Bersarinplatz as it is today (empty).PNG | plaza-today.png |
| Kolonialkarte_1884_2.jpg | colonial-map.jpg |
| Das deutsch-ostafrikanische Schutzgebiet S. 137 Kilimanjaro von Moshi.png | kilimanjaro-from-moshi.png |
| Deutsche Emin-Pascha Expedition S. 41 Ankunft Strand.png | landing-on-the-coast.png |
| Deutsche Emin-Pascha Expedition S. 57 Zelte.png | expedition-camp.png |
| Das deutsch-ostafrikanische Schutzgebiet S. 297 Daressalam.png | dar-es-salaam.png |
| Deutsche Emin-Pascha Expedition S. 129 Auseinandersetzung.png | using-force.png |
| Deutsche Emin-Pascha Expedition S. 21 Carl Peters.png | carl-peters.png |
| Das deutsch-ostafrikanische Schutzgebiet S. 132Moshi Militärstation+.png | moshi-military-station.png |
| Der Kolonialbrunnen Satire with Carl Peters.jpg | kolonialbrunnen.jpg |
| Pariser_Platz,_Berlin_1900_(2).jpg | pariser-platz-1900.jpg |
| Competition Monument Draft Hermann Hahn & Carl Sattler.jpg | design-hahn-sattler.jpg |
| Competition Monument Draft Adolph Brütt.jpg | design-bruett.jpg |
| Competition Monument Draft Adof Brütt (landscape).jpg | design-bruett-landscape.jpg |
| Competition Monument Draft Georg Wrba (landscape).jpg | design-wrba.jpg |
| Competition Monument Draft Ludwig Cauer.jpg | design-cauer.jpg |
| Competition Monument Draft Elephant Winner / Fritz Behn.jpg | design-behn.jpg |
| Newspaper article with elephant winning draft.jpg | newspaper-1914.jpg |
| 1932_Eröffnung_Elephant.jpg | elephant-opening-1932.jpg |
| Elefant_mit_Inschrift_Unsere_Kolonien.jpg | elephant-unsere-kolonien.jpg |
| Reichskanzler Theobald von Bethmann-Hollweg während seiner Rede vor dem Reichstag am 4. August 1914 (pa/akg).jpg | reichstag-1914.jpg |
| VERSAILLER_VERTRAG_03.jpeg | versailles-protest-1919.jpg |
| elefant-denkmal-antrag.jpg | application-1926.jpg |
| Kolonialausstellung8.jpg | colonial-exhibition-1935.jpg |
| Antikolonialdenkmal_Bremen_-msu-2022-9798-.jpg | elephant-today.jpg |
| 2011 charite herrero nama kontaktaufnahme ancestors.png | charite-2011.png |
| 2014 2014 charite völkermord verjährt nicht.png | charite-2014.png |
| 2018 völkermord verjährt nicht gendarmenmarkt protest.png | gendarmenmarkt-2018.png |
| apologies and reparations for colonization protest 2004 120 jahrestag konkokonferenz.png | protest-2004.png |
| Renamed street picture.jpg | mohrenstrasse-sign.jpg |
| decolonize berlin auf bismarckstatue.png | decolonize-berlin.png |
| Antikolonialdenkmal_Bremen-für menschenrechte gegen apartheid.jpg | anticolonial-monument.jpg |
| Antikolonialdenkmal_Bremen_Ohamakari_Tafel.jpg | ohamakari-plaque.jpg |
| Antikolonialdenkmal_Bremen_insignia1.jpg | monument-detail-1.jpg |
| Antikolonialdenkmal_Bremen_insignia2.jpg | monument-detail-2.jpg |
| nelson mandela park vor elephant.jpg | nelson-mandela-park.jpg |

Not used any more: the first Kilimanjaro picture (S. 113), both steamers, the second confrontation (S. 233), the landscape scene (S. 97), the second view of Behn's design, `Antikolonialdenkmal_HB2013.jpg` and `Elephant Statue in Bremen today.jpg`.

Large photos (over about 1 MB) are worth shrinking before uploading, for example with squoosh.app, so the page loads quickly on phones.

## Editing

- **Captions, hover texts and credits:** in `index.html`, search for `var SLOTS`. Each picture has `title` (caption), `hover` (text near the cursor), `short` (credit under the picture) and `full` (entry in the image credits).
- **Footnotes:** search for `var NOTES`. They are numbered as in the essay.
- **Map flight:** open the page with `?mapdebug` added to the address, scroll to the map and click on Germany and on Kilimanjaro. Copy the two x/y pairs into `MAP_FROM` and `MAP_TO` near the top of the script.
