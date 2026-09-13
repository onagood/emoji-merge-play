# Meadow artwork

17 retained original illustrations generated for this game with the built-in OpenAI
image generation tool on 2026-09-13. They are separate from Twemoji artwork.

The source PNGs are preserved in `art-source/meadow/*-generated.png` in the
development project. Exact prompts: `tools/meadow-generation.json`.
`tools/prepare-meadow.py` crops extraction padding, preserves aspect ratios,
exports transparent WebP sprites and square shop icons, and partitions the
butterfly and bee into aligned layers for animation. No third-party stock
illustrations were added. Crop dimensions: `art-source/meadow/preparation.json`.

Scene and icon variants share the same original. Shop upgrades reuse the
matching cloud illustration. Grass, clover and flowers now use new repeating
painted textures in `assets/lawn/`; see that folder's `PROVENANCE.md`.
At the user's request, the four isolated plant illustrations, their icons,
two seasonal grass variants and baked ground/flower bands were removed.

The second batch adds 9 originals (8 more shop items): poppies/cornflowers,
tractor, pickup, delivery truck, helicopter, lantern, old tree, hot-air balloon
and snowman. Source PNGs: `art-source/meadow-expansion/`; generation prompts:
`tools/meadow-expansion-generation.json`. Technical preparation:
`tools/prepare-meadow-expansion.py`. Wheel pivots and contact positions were
measured in `tools/meadow-pivots.json`; the game uses the
generated `src/meadow-geometry.js`. Six complete vehicle wheels, three separate
stationary bodies and wheel wells, and the two helicopter layers share the
original canvas alignment. Hidden tire sections reuse
reflected pixels from the visible lower tread; the fenders remain stationary.

The balloon received a background-cleanup edit with ImageGen. Its neutral
checkerboard was then removed programmatically, as authorised by the user;
both generated versions are preserved. The exported image was checked on a
blue background. The spooky world's bare tree remains its original SVG.

Four retained autumn/winter variants of bush and old tree were generated with
the built-in ImageGen tool on 2026-09-13. Prompts and input references:
`tools/meadow-seasons-generation.json`. Source PNGs are kept locally in
`art-source/meadow-seasons/`. The generated grass variants were subsequently
removed along with the isolated summer plants.

`tools/prepare-meadow-seasons.py` exports these variants and the paired cloud
icon. The exporters skip retired plants and no longer bake ground bands.
Runtime raster icons are 96 px; scene sizes follow their actual display sizes.
All PNG masters stay outside Git tracking; their hashes and sizes are recorded
in `tools/meadow-source-manifest.json`. Rebuild/archive instructions:
`art-source/shop/MEADOW-ARCHIVE.md`.
