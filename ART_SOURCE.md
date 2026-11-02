# Idle Anime Fighters — Art Source Guide

## Visual target
A high-energy, classic 2D anime fighting-game look strongly informed by MUGEN presentation: expressive poses, readable silhouettes, dramatic hit-stop, impact flashes, knockback, energy effects, and richly illustrated stages. The goal is an arcade fighter that happens to have incremental progression, not a generic idle game.

## Prototype asset sourcing
- For private concept evaluation, MUGEN and community fighter sprites may be used when the user supplies the pack or it is lawfully accessible for the intended use.
- Track every external pack in `ASSET_CREDITS.md`, including author, source URL, license/terms, attribution, and modifications.
- A public repository can redistribute only assets whose license or permission allows it. Personal/private play does not automatically authorize publishing copyrighted sprite files in a public repo.
- If a desired pack cannot be redistributed, keep it local or private and do not commit it publicly.
- The current prototype integrates three complete CC0 animated fighter packs as the character foundation. The presentation, HUD, arena staging, and combat effects should evoke classic MUGEN arcade fighters. Do not use emoji, colored rectangles, stick figures, or generic icons as fighter substitutes.

## Implemented fighter sprite sets
- Kai Ren: LuizMelo's Martial Hero animation set (idle, run, jump, fall, two attacks, hit, death).
- Raika: LuizMelo's Martial Hero 2 animation set (idle, run, jump, fall, two attacks, hit, death).
- Yurei: LuizMelo's Huntress animation set (idle, run, jump, fall, attack, hit, death).
- These are game-ready animated sprite strips rather than native MUGEN SFF character archives; the project adapts them to its own combat simulation and uses the MUGEN presentation style around them.

## Character sprite requirements
- Prefer complete sprite sheets or frame sequences with transparent backgrounds, consistent frame dimensions, stable feet baselines, and clear frame naming.
- Include idle, walk/run, light/heavy attack, special, hurt, knockback, and defeat states where the source pack provides them.
- Preserve character scale, anatomy, costume details, and facing direction. Flip only after checking asymmetric details.
- Read silhouettes at actual in-game size and against the stage palette.
- Integrate authentic frame sequences rather than stretching one idle pose to fake a full moveset.

## Combat VFX
- Make hits feel forceful through layered impact bursts, slash arcs, speed lines, dust puffs, hit sparks, brief hit-stop, camera shake, and controlled screen flashes.
- Energy attacks need distinct projectile/beam visuals, charging cues, travel behavior, impact effects, and cooldown feedback.
- Effects must communicate attack strength and direction without obscuring the fighters for long periods.

## Stage art
- Side-view fighting stages with a clear floor plane and enough horizontal room for spacing, dashes, and knockback.
- Build depth with a foreground fighting plane, midground architecture/terrain, and distant scenery.
- Stage palettes should contrast with fighter palettes and effects.

## UI art
- UI should feel like an arcade fighting game: compact status panels, sharp borders, restrained metallic or energy accents, clear labels, and bold readable numbers.
- Health and energy bars must be legible during action.
- Buttons and panels must remain usable on desktop and touch screens. The arena should occupy the largest share of the play screen.

## Quality gate before commit
- Inspect sprite alignment, transparency, silhouette readability, animation continuity, and facing direction.
- Check effects against light and dark stage areas.
- Confirm all referenced assets exist and load; no broken paths or missing frames.
- Play through the relevant combat states and verify that animation transitions do not pop, freeze, or show incorrect frames.
- Only commit finished, integrated assets and working code. No placeholder art or unfinished sprite sheets.
