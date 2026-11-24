# AudioScape music and sound effects

Free music and sound effects that [AudioScape](https://github.com/Joejibobo) plays under audiobooks and read-aloud books. Everything here is **CC0 1.0** (Creative Commons Zero) or **public domain**, so anyone may use it for any purpose without asking or crediting.

## What's here

- `catalog.json`: the music catalog AudioScape reads (17 tracks, about 50 minutes). For each track it lists the title, artist, duration, the styles and moods it suits, a loudness correction (`gainDB`), an analysis made in advance (tempo, key, loudness, energy, a loudness curve at one value a second), the licence and where it came from, and the file's address, size and SHA-256.
- `effects.json`: 30 sound effects (thunder, rain, doors, footsteps, swords, bells, clocks, a wolf and more) with their kind, length, the time of their loudest moment (`peakOffset`), level trim, SHA-256, licence and source.
- `LICENSES.md`: every item with its author, source page, the licence wording on that page, the date it was read and a link to the saved page.
- `evidence/`: the source pages as they were downloaded, kept as proof of the licence at the time (with the sites’ own map keys blanked out).
- The audio is attached to the [v1 release](https://github.com/Joejibobo/audioscape-music/releases/tag/v1) (AAC in `.m4a`: music at 128 kbps, effects mono at 96 kbps); the manifests' `baseURL` points there.

## Licences in short

- Music from Wikimedia Commons: Kimiko Ishizaka's Bach recordings (CC0), Robin Alciatore's Satie and Musopen's Grieg (released into the public domain by the performers), Musopen's Mendelssohn (Public Domain Mark by the copyright holder). The compositions are long out of copyright.
- Music from the Free Music Archive (HoliznaCC0, Maarten Schellekens) and Freesound (SG80_MED1A, neolein, szegvari, MrPork, Romariogrande): CC0 1.0, marked by the artist. None of the chosen tracks is marked as AI-generated.
- Sound effects: all from Freesound, each marked CC0 1.0 by its uploader.

Freesound originals need an account to download, so the Freesound items were made from the high-quality previews each page offers publicly. Files were trimmed of long silences, converted to AAC and, for effects, normalised to −3 dBFS; quiet music was raised once before encoding, and loud music carries a negative `gainDB` the player applies (target −18 LUFS).

CC0 and public domain need no credit, but Musopen and neolein ask for one as a courtesy: thank you to them and to every artist listed in `LICENSES.md`.
