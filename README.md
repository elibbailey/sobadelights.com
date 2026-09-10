# sobadelights.com

The landing page for SOBA, makers of interesting consumer goods.

Plain static site: `index.html` is the whole page (styles and the morphing-object script are inline),
`404.html` is the not-found page. No build step. Served by GitHub Pages from the `main` branch;
`CNAME` pins the custom domain.

To change the copy, edit `index.html`. To add or reorder the objects the silhouette morphs through,
edit the `SHAPES` list near the bottom of `index.html`: each entry is a closed outline drawn in a
100×100 box (y grows downward), a catalog code, and a caption.

## Palette notes

The light "paper" colour is `--paper` in `index.html` (also used in `404.html`, `og.html`, `icon.html`).
It is currently `#f8d5a5`, a light salmon-yellow chosen to match how the page looked through f.lux.
Other options that were considered, for a quick swap (keep the two `rgba(...)` variables next to it in step):

| Option | Hex | Notes |
|---|---|---|
| Current: light salmon-yellow | `#f8d5a5` | 5.9:1 on the blue |
| f.lux Halogen 3400K on the original cream | `#f6b976` | warmer tan, 4.8:1 |
| f.lux 2700K | `#f6a34f` | 4.0:1, too low for body text |
| f.lux Candle 1900K | `#f67c00` | 3.1:1, clashes with the orange button |
| Original cream | `#f6f0e1` | the untinted design |

`og.png` and `apple-touch-icon.png` are rendered from `og.html` and `icon.html`: open the page, call
`renderCard()` / `renderIcon()` in the console, and save the returned PNG blob (the pages include a
`postTo` helper that sends it to a local receiver on port 8766).
