# Original painted lawn patterns

Six new source images created for this project using the built-in OpenAI
image generation tool on 2026-09-13: summer, autumn and winter grass, clover,
daisies, and poppies/cornflowers. The original demo informed the repeated
coverage and scale; its SVG strokes are not the artwork in these WebP tiles.

Exact prompts: `tools/lawn-generation.json`.
Source hashes: `tools/lawn-source-manifest.json`.
Reproducible technical preparation: `tools/prepare-lawn.py` (Pillow and numpy).

Preparation removes near-transparent extraction noise, crops complete generated
marks, proportionally resizes them and composes irregular repeating tiles.
Marks crossing an edge are also composited on the opposite edge. No new plant
shapes are drawn programmatically. Shop icons are swatches of these tiles.

On 2026-09-14 the regular rows were replaced with seeded random placement with
minimum distances measured across tile boundaries. Each plant varies in size,
mirroring and tilt; clover may rotate freely. Layer seeds differ so flowers do
not line up with grass. Larger repeat periods preserve the plant display scale.
Positions are baked once, not randomized during gameplay.

Release: six 384 x 384 transparent WebP tiles and six 96 x 96 icons, 137,294 bytes.
Grass density changes repeat spacing; clover and flowers are separate repeating
layers. Seasonal grass uses separately generated illustrations. Night uses the
existing scene lighting. No per-plant elements or animations are added.

PNG masters and large previews are in the ignored local `art-source/lawn/`
folder, excluded from the release and Git. Archive that folder separately.
