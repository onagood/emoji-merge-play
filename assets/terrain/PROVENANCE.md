# Seasonal terrain

Eight original terrain paintings generated with built-in ImageGen on 2026-09-14:
one hill panorama and one ground surface for each of spring, summer, autumn,
and winter. The approved four-season concept is the style reference. No sky,
sun, fence, tree or other scene decoration is baked into these runtime images.

Prompts and source paths: `tools/terrain-generation.json`.
Local PNG masters: `art-source/terrain/` (excluded from Git and the game build).
Technical exports: `tools/prepare-terrain.py`; transparent background cleanup,
WebP compression, a seamless vertical ground join, and alpha skyline samples
for existing sheep/vehicle paths. No new painting is produced programmatically.

The ground remains covered continuously. Existing purchased flower/clover
details are layered separately, so the shop progression remains functional.
