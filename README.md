# CDG Karaoke

![CDG Karaoke specimen](specimen.png)

A color pixel font that reproduces the lyric type from a CD+G karaoke disc. Words
not yet sung are white, and each word fills in as it is sung. Music notes stay
white. It ships with two color palettes so a renderer can flip a word from unsung
to sung.

## Files

- `CDGKaraoke.otf`, `CDGKaraoke.ttf` for desktop
- `CDGKaraoke.woff2`, `CDGKaraoke.woff` for web

## How it works

It is a color font (COLR/CPAL): one file, two palettes. Palette 0 is the sung
state, palette 1 is the unsung state. Switch per word with CSS `font-palette`, or
a renderer's palette selection, to make a line wipe from one to the other. The four
music notes (U+2669 to U+266C) stay white in both palettes.

Charset is ASCII printable plus the four notes. There is no variable axis; the
color is carried by the palettes, so it renders in any COLR-capable app.

## Base font

Drawn from NimbusRoman-Bold (URW Core 35 v2.0), a Times clone under the SIL Open
Font License with no reserved font name. It was rasterized onto the CD+G pixel grid
with hinting and antialiasing off, then squared to match the disc.

## License

SIL Open Font License 1.1. See `OFL.txt`. Free to use, embed, study, modify, and
redistribute. The fonts carry no embedding restrictions (fsType 0).
