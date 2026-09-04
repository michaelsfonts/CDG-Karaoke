# CDG Karaoke

![CDG Karaoke specimen](specimen.png)

The words on an old karaoke screen, turned into a font. White until you sing them,
then they fill in, one word at a time, the way the machine paints the line.

## Two palettes

It is a color font with two palettes built in. One paints a word cyan for sung, the
other white for not sung yet. A karaoke player flips a word from white to cyan as
you sing it, so the color sweeps across the line. The music notes stay white in
both. It opens on the cyan palette, so it just shows up in any app that does color
fonts, nothing to turn on.

To switch palettes in a browser:

    @font-palette-values --sung   { font-family: "CDG Karaoke"; base-palette: 0; }
    @font-palette-values --unsung { font-family: "CDG Karaoke"; base-palette: 1; }

Then put `font-palette: --sung` or `--unsung` on the text. Entry 2 is the letter
fill, entry 3 is the notes.

## Files

- `CDGKaraoke-Regular.otf`, `CDGKaraoke-Regular.ttf` for desktop
- `CDGKaraoke-Regular.woff2`, `CDGKaraoke-Regular.woff` for the web

To install, open the `.otf` or `.ttf` and hit Install. Release ZIPs are on the
[Releases](https://github.com/michaelsfonts/CDG-Karaoke/releases) page.

## Where the letters came from

I started with Nimbus Roman Bold, a free Times knockoff. Dropped each letter onto
the chunky karaoke pixel grid, killed all the smoothing, and squished it a bit.

## License

Free under the SIL Open Font License. Use it, embed it, change it, pass it around.
See `OFL.txt`.
