# 0002 Zero Vector EGA Rendering

## Context
1987 Lucasfilm games used authentic EGA pixel art, not modern geometric primitives.

## Decision
Strict Zero Vector Policy. All character sprites, rooms, objects, and door overlays must use 16-color EGA raster graphics. Canvas `fillRect`/`arc` are banned for game visual elements.

## Consequences
Guarantees authentic retro aesthetic and eliminates visual regressions.
