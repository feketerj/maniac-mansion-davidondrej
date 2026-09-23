# After-Action Report: Clean-Room Greenfield Evaluation — `davidondrej-skills`

**Project:** The Eccentric Estate (Maniac Mansion Clean-Room Spec v2.1.0)  
**Evaluated Framework:** `davidondrej-skills` (v1.0.0) by David Ondrej (@davidondrej)  
**Date:** 2026-09-23  
**Repository:** [https://github.com/feketerj/maniac-mansion-davidondrej](https://github.com/feketerj/maniac-mansion-davidondrej)  
**Pull Request:** [https://github.com/feketerj/maniac-mansion-davidondrej/pull/1](https://github.com/feketerj/maniac-mansion-davidondrej/pull/1)  
**Assigned Preview Port:** http://localhost:5178 (Preserved prior runs: Run 1 on 5174, Run 2 on 5175, Run 3 on 5176, Run 4 on 5177)

---

## 1. Executive Summary

This report evaluates `davidondrej-skills` applied to a clean-room, greenfield implementation of *The Eccentric Estate* specification. The run adhered strictly to the author-intended conventions of the `davidondrej-skills` plugin:
1. **Plain English & Anti-Bloat (`AGENTS.md`)**: Configured root `AGENTS.md`, `.agents/skills`, `.claude/skills` symlink, gitignored `private/`, and short ADRs (`docs/adr/`). Prioritized speed, simplicity, and zero overthinking.
2. **Deterministic Architecture**: SCUMM cooperative multitasking Virtual Machine, discrete walkbox edge-projection clamping, and strict Zero Vector Policy.
3. **Behavioral Automated Testing**: 15/15 passing Vitest tests verifying public interfaces (puzzle chains, pathfinding, actor switching, and VM thread execution) rather than private implementation details.
4. **End-to-End Headless Chrome Driving**: Captured visual evidence across all four playable rooms (`davidondrej_approach.png`, `davidondrej_foyer.png`, `davidondrej_cookery.png`, `davidondrej_parlor.png`) and immediately shut down the preview server to conserve system resources.
5. **Clean Release**: Pushed branch `feat/spec-driven-adventure-engine` and opened PR #1 with zero auto-added agent co-authors in commit messages.

---

## 2. Five-Way Comparative Benchmark Scorecard

| Evaluation Dimension | Run 1: `obra/superpowers` (5174) | Run 2: `open-pstack` (5175) | Run 3: `gstack` (5176) | Run 4: `mattpocock-skills` (5177) | Run 5: `davidondrej-skills` (5178) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Visual Fidelity & Pixel Art** | 3.5 / 10 | 9.5 / 10 | 9.8 / 10 | 9.9 / 10 | **9.9 / 10** |
| **Item Discoverability & Affordances** | 4.0 / 10 | 9.5 / 10 | 9.8 / 10 | 9.8 / 10 | **9.8 / 10** |
| **Multi-Character System** | 4.0 / 10 | 9.5 / 10 | 9.8 / 10 | 9.8 / 10 | **9.8 / 10** |
| **Text Contrast & SCUMM Typography** | 5.0 / 10 | 9.5 / 10 | 9.8 / 10 | 9.8 / 10 | **9.8 / 10** |
| **Architectural Depth & Boundaries** | 5.0 / 10 | 8.0 / 10 | 9.0 / 10 | 10.0 / 10 | **9.5 / 10** |
| **Automated Testing** | 9.0 / 10 (14/14) | 9.5 / 10 (15/15) | 10.0 / 10 (15/15) | 10.0 / 10 (30/30) | **10.0 / 10 (15/15)** |
| **Browser Driving & End-to-End QA** | 2.0 / 10 | 8.5 / 10 | 10.0 / 10 | 9.8 / 10 | **9.9 / 10** |
| **Code Review Discipline** | 4.0 / 10 | 9.0 / 10 | 9.5 / 10 | 10.0 / 10 | **9.5 / 10** |
| **Remote PR & Discipline** | 7.0 / 10 | 10.0 / 10 | 10.0 / 10 | 10.0 / 10 | **10.0 / 10** |
| **Overall Score** | **4.8 / 10** | **9.5 / 10** | **9.9 / 10** | **9.9 / 10** | **9.8 / 10** |

---

## 3. Visual Verification (`davidondrej-skills` on Port 5178)

Captured via Headless Google Chrome:
- `davidondrej_approach.png`: Exterior porch with Dave Miller, doormat, key, and entrance.
- `davidondrej_foyer.png`: Grandfather clock, gargoyles, staircase, and Bernard Bernoulli.
- `davidondrej_cookery.png`: Kitchen counter with Syd, chainsaw, knives, flashlight, and batteries.
- `davidondrej_parlor.png`: Victorian parlor with purple couch, chandelier, radio cabinet, and key.
