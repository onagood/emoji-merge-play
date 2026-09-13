# Animals artwork

Eleven soft toy body illustrations generated for Plopmoji with the built-in
imagegen tool on 2026-09-13, based on the concept sheet approved in this task.
They are not Twemoji artwork. The character order is Ladybug, Hamster, Frog,
Chick, Chicken, Bunny, Kitty, Puppy, Panda, Unicorn, Lion.

The user explicitly authorised programmatic background removal, alignment
and transparent PNG/WebP export. The generated RGB originals contained a
checkerboard backdrop; `tools/prepare-animals.py` prepares the delivery files.
Exports preserve the original aspect ratio with one scale for both axes;
width and height are not independently stretched to fill a square.
Original generated files are retained in `art-source/animals/`, outside the
release manifest. Exact per-character generation prompts and the reference
path are recorded in `tools/animal-generation.json`.

Body textures contain cheeks, noses/beaks and species markings. Eyes and
mouths are original runtime canvas drawings in `src/animals.js`. Blinking,
neighbour glances and impact expressions are visual effects only.
