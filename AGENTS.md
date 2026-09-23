# AGENTS.md — The Eccentric Estate (David Ondrej Edition)

## Rules
- Make ALL responses clear & concise. Plain English, short sentences.
- Avoid overthinking at all cost. Prioritize working fast and moving fast.
- Focus on code quality, simplicity, robustness, and scalability.
- Keep dependencies minimal and standard.
- Zero Vector Policy: authentic 16-color EGA raster art, 12-frame 4-way walk cycles. No geometric vector fallbacks.
- Behavior-focused automated tests over private implementation tests.
- Verify end-to-end visuals with headless Chrome before shipping.

## Architecture
- `src/engine/`: SCUMM VM, NavMesh edge-projection clamping, Actor walk cycles, Room state, Audio synthesizer, Canvas 320x200 renderer.
- `tests/`: Behavioral tests verifying puzzle chains, pathfinding, actor switching, and VM threads.
- `docs/adr/`: Architectural Decision Records.
