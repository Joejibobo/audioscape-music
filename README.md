# AudioScape music and sound effects

Free music and sound effects that [AudioScape](https://github.com/Joejibobo) plays under audiobooks and read-aloud books. Everything here is **CC0 1.0** (Creative Commons Zero) or **public domain**, so anyone may use it for any purpose without asking or crediting.

## What's here

- `catalog.json`: the music catalog AudioScape reads (version 2: 160 tracks, about 9 hours, 535 MB, across 16 styles and 5 moods). For each track it lists the title, artist, duration, the styles, moods and kinds of scene it suits, a loudness correction (`gainDB`), an analysis made in advance (tempo, key, loudness, energy, a loudness curve at one value a second), the licence and where it came from, and the file's address, size and SHA-256.
- `effects.json`: 30 sound effects (thunder, rain, doors, footsteps, swords, bells, clocks, a wolf and more) with their kind, length, the time of their loudest moment (`peakOffset`), level trim, SHA-256, licence and source.
- `LICENSES.md`: every item with its author, source page, the licence wording on that page, the date it was read and a link to the saved page.
- `evidence/`: the source pages as they were downloaded, kept as proof of the licence at the time (with the sites’ own map keys blanked out).
- The audio is attached to releases (AAC in `.m4a`: music at 128 kbps, effects mono at 96 kbps): the 17 first tracks and the effects to [v1](https://github.com/Joejibobo/audioscape-music/releases/tag/v1), the 143 tracks added in version 2 to [v2](https://github.com/Joejibobo/audioscape-music/releases/tag/v2). `catalog.json`'s `baseURL` is the v2 release and the v1 tracks carry absolute v1 URLs; `effects.json` points at v1.

## Licences in short

- Music from Wikimedia Commons: Kimiko Ishizaka's Bach recordings (CC0), Robin Alciatore's Satie and Musopen's Grieg (released into the public domain by the performers), Musopen's Mendelssohn (Public Domain Mark by the copyright holder). The compositions are long out of copyright.
- Music from the Free Music Archive (HoliznaCC0, Maarten Schellekens) and Freesound (SG80_MED1A, neolein, szegvari, MrPork, Romariogrande): CC0 1.0, marked by the artist. None of the chosen tracks is marked as AI-generated.
- Sound effects: all from Freesound, each marked CC0 1.0 by its uploader.

### Added in version 2

- Wikimedia Commons: United States Air Force, Marine, Navy and Army band recordings (works of the US federal government, public domain; compositions traditional, out of copyright, or written by band members), Musopen orchestra and quartet recordings released by Musopen (Brahms, Grieg, Borodin, Haydn, Dvořák, Mendelssohn, Beethoven), Kimiko Ishizaka's CC0 Bach, Swedish folk fiddle recordings from Svenskt visarkiv (CC0 by the Swedish Performing Arts Agency), performers' own public-domain releases (Chopin nocturnes by Frank Lévy, Satie, Fauré, Alberti), US recordings published before 1925, and CC0 tracks by John Bartmann, Loyalty Freak Music and Rafael Krux (FreePD).
- Free Music Archive: CC0 tracks by HoliznaCC0, John Bartmann, Komiku, Ondrosik, TRG Banks, Koi-discovery, Twelvety9, Zane Little, Lucas Gonze, xik, Monplaisir, Art Flower and others, and public-domain piano rolls; each page's licence line, “AI generated?” (only “No” taken) and “Instrumental” were read and saved.
- Internet Archive: three lute recordings by David-Sky Marchant, marked CC0 on his own items.
- Not taken: anything CC BY or BY-SA, Pixabay/Mixkit/Uppbeat-style licences, AI-generated tracks, old European recordings marked only {{PD-EU-audio}} (still protected in the US), public-domain compositions in copyrighted recordings, and third-party Internet Archive uploads. Freesound was not searched for version 2.

Freesound originals need an account to download, so the Freesound items were made from the high-quality previews each page offers publicly. Files were trimmed of long silences, converted to AAC and, for effects, normalised to −3 dBFS; quiet music was raised once before encoding, and loud music carries a negative `gainDB` the player applies (target −18 LUFS).

CC0 and public domain need no credit, but Musopen and neolein ask for one as a courtesy: thank you to them and to every artist listed in `LICENSES.md`.
