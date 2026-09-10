# sobadelights.com

The landing page for SOBA, makers of interesting consumer goods.

Plain static site: `index.html` is the whole page (styles and the morphing-object script are inline),
`404.html` is the not-found page. No build step. Served by GitHub Pages from the `main` branch;
`CNAME` pins the custom domain.

To change the copy, edit `index.html`. To add or reorder the objects the silhouette morphs through,
edit the `SHAPES` list near the bottom of `index.html`: each entry is a closed outline drawn in a
100×100 box (y grows downward), a catalog code, and a caption.
