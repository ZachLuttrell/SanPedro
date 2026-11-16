# SanPedro

An endless Sonoran desert to wander and survive in, live at
[sanpedrorivervalley.netlify.app](https://sanpedrorivervalley.netlify.app).

`index.html` is the whole game: a single page, no build step. It draws the valley in 3D and
lets you switch at any time between a smooth mesh and a voxel world (`V`). Both are stood up
from the same map. three.js loads from a CDN, so the page needs a network connection.

## Playing

| Key | Does |
| --- | --- |
| `WASD` / arrows | move (relative to where you look) |
| drag / wheel | look / zoom (all the way in for first person) |
| `Shift` | jog |
| `E` | use or gather whatever the prompt names: drink, chop, pick, catch, cook, sleep |
| `F` | eat |
| `B` | build: campfire, ramada, water olla, bedroll |
| `C` | stake a claim (a home point until you have a bedroll) |
| `V` | voxel / mesh |
| `T` | hurry the sun |
| `M` | sound on / off |

On a phone, the left thumb moves, the right thumb looks, and the buttons do the rest.

## Earlier versions

- `classic/wander-2d.html` — the first top-down version: wandering only.
- `classic/survival-2d.html` — the top-down version that introduced thirst, hunger, body
  heat, gathering, building and sound. The 3D game carries all of that over.

The river, elevation, biome and plant functions are the same in all three, so it is the same
valley in each. The 3D game keeps a share of the 2D plants (same tiles, fewer of them),
because the 2D densities close into a wall of cactus once plants have real height.
