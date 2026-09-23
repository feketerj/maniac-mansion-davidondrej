# 0001 SCUMM Modular Architecture

## Context
Recreating Maniac Mansion requires robust pathfinding, cooperative script execution, multi-character state, and sentence grammar composition.

## Decision
Modular engine separation across NavMesh, ActorManager, RoomManager, VirtualMachine, AudioSystem, and Renderer.

## Consequences
Behavior can be tested cleanly without coupling to internal canvas rendering state.
