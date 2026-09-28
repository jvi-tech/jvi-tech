# JVI-TECH UI47 — Google AI Studio / GitHub Analysis Repository

Purpose: bounded analysis package for converting the original FYT UI47 launcher into the JVI-TECH launcher by modifying the existing launcher rather than creating a new launcher architecture.

## Important
This is an analysis repository, not yet a buildable Android Studio project.

The original APK and decoded resources are included so an AI agent can inspect the existing launcher structure.

Do NOT:
- rewrite FYT/SYU services without evidence;
- change package/sharedUserId/HOME behavior casually;
- build a new launcher architecture;
- modify files before completing Phase 1 analysis.

## Contents
- `00_ORIGINAL/` — original UI47 APK
- `01_DECODED_RESOURCES/` — decoded XML resources
- `02_DEX_ANALYSIS/` — classes.dex plus class/string/layout inventories
- `03_TARGET_LAYOUTS/` — key Home layouts and resolution variants
- `04_KEY_ASSETS/` — key UI assets
- `05_UI47_MAPPING/` — component mapping and preliminary report
- `AI_STUDIO_PHASE1_PROMPT.md` — first analysis prompt

## Target
The desired interface is represented by a separately attached JVI-TECH Launcher MASTER V1 image.

## Next step
Import this repository into Google AI Studio Build mode via `Add files (+) -> Import from GitHub`, then attach the MASTER V1 image and send `AI_STUDIO_PHASE1_PROMPT.md`.

Do not ask the agent to modify or build the APK yet.
