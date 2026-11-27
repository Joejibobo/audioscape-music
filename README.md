# AudioScape music and sound effects

Free music and sound effects that [AudioScape](https://github.com/Joejibobo) plays under audiobooks and read-aloud books. Everything here is **CC0 1.0** (Creative Commons Zero) or **public domain**, so anyone may use it for any purpose without asking or crediting.

## What's here

- `catalog.json`: the music catalog AudioScape reads (version 4: 195 tracks, about 11 hours, 645 MB, across 16 of its 17 styles and 5 moods). For each track it lists the title, artist, duration, the styles, moods and kinds of scene it suits, a loudness correction (`gainDB`), an analysis made in advance (tempo, key, loudness, energy, a loudness curve at one value a second), the licence and where it came from, and the file's address, size and SHA-256.
- `effects.json`: 30 sound effects (thunder, rain, doors, footsteps, swords, bells, clocks, a wolf and more) with their kind, length, the time of their loudest moment (`peakOffset`), level trim, SHA-256, licence and source.
- `LICENSES.md`: every item with its author, source page, the licence wording on that page, the date it was read and a link to the saved page.
- `evidence/`: the source pages as they were downloaded, kept as proof of the licence at the time (with the sites’ own map keys blanked out).
- The audio is attached to releases (AAC in `.m4a`: music at 128 kbps, effects mono at 96 kbps): the 17 first tracks and the effects to [v1](https://github.com/Joejibobo/audioscape-music/releases/tag/v1), the 143 tracks added in version 2 to [v2](https://github.com/Joejibobo/audioscape-music/releases/tag/v2), the 35 added in version 3 to [v3](https://github.com/Joejibobo/audioscape-music/releases/tag/v3). `catalog.json`'s `baseURL` is the v3 release and the v1 and v2 tracks carry absolute URLs to their own releases; `effects.json` points at v1.

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

### Added in version 3

- Wikimedia Commons: Grieg's Holberg Suite by the United States Marine Chamber Orchestra and Holst's Mercury and Uranus by the US Air Force Heritage of America Band (federal works), Norwegian Hardanger fiddle and Swedish nyckelharpa and fiddle recordings from Svenskt visarkiv (CC0), Lucas Gonze (CC0), The Rogue Bluegrass Band (released into the public domain by the band), and two recordings published before 1926, public domain in the US by age: Imdad Khan's sitar (1904) and Gilliland and Robertson's Arkansaw Traveler (1922).
- Free Music Archive: CC0 tracks by John Bartmann (Western Skies, Underwater Wonders), HoliznaCC0, Ondrosik and TRG Banks.
- Every new file was also run through Apple's sound classifier to keep out speech and singing. Not taken: synthesizer and MIDI renderings of medieval and other pieces, 1901–1903 field cylinders too noisy to play under narration, and a 1942 Scheherazade marked CC0 by an uploader who could not own it.

### Version 4 (labels only)

Same audio, files and addresses as version 3. Every track was relabelled by hand: symphonies, overtures, suites and quartets carry the classical style (`regencyClassical`, plus the world they belong to, such as `norse` for Grieg's Peer Gynt and Holberg Suite), concert-band pieces and marches carry `military`, and `epicFantasy` stays only on cinematic and game-like pieces (Komiku, Ondrosik, SG80). Each track also gained optional labels in `tags`: `character` (filmScore, game, ambient, classical, band, folk, electronic, jazz, choral, weighted 0–1), `instruments` (up to five), `places` (up to four settings it evokes), `era` (historical or modern) and `shape` (steady, builds, swells or sparse, from the loudness curve). The loudness curve is rounded to 0.1 dB, which halves the manifest.

## Ambience

- `ambience.json`: field-recording beds (rain, wind, sea, fire, crowd, city, night, interior, forest, water, battle) that AudioScape loops under narration. Each entry has the bed, title, length, a level trim (`gainDB`), the file's address, size and SHA-256, and its licence and source. The audio (AAC 128 kbps, 44.1 kHz, about −28 LUFS, true peak ≤ −3 dBTP, each file a seamless loop) is in release [ambience-v1](https://github.com/Joejibobo/audioscape-music/releases/tag/ambience-v1); licences and saved source pages are listed in `LICENSES.md` under “Ambience”.
