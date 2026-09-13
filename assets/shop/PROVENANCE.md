# Shop illustrations

Created for this project on 2026-09-13 with the built-in OpenAI image generation
tool: five box illustrations and seven weather/star illustrations. The existing
project meadow contact sheet was a style reference. These are separate from
Twemoji artwork.

Exact generation prompts: `tools/shop-art-generation.json`.
Original source hashes: `tools/shop-art-source-manifest.json`.
Technical preparation: `tools/prepare-shop-art.py`.
Reviewed material crop coordinates: `tools/shop-art-materials.json`.

Preparation preserves the original drawings: alpha cropping, proportional
resizing and WebP encoding. A neutral checkerboard baked into the dark oak
source was removed using its low chroma. Strong wind is a denser composition
of the generated breeze illustration. Five repeating material tiles are sampled
from the box front panels and mirrored at their edges.

Runtime files: thirteen transparent 96 x 96 icons and five 128 x 128 material
tiles, 46,530 bytes in total. Box textures cover only the established external
frame; game field and physics dimensions are unchanged.

PNG masters and larger gallery previews are stored in the ignored local folder
`art-source/shop-batch/`, outside the release. Archive this folder separately
before moving to another machine; the source manifest alone cannot reproduce
the original generated pixels.
