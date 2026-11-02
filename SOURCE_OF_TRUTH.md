# Idle Anime Fighters — Source of Truth

## Project identity
A browser-based incremental anime fighting game. The arena is the centerpiece: purchased fighters spawn into a 2D side-view fighting stage and automatically battle when opponents are present. The player earns currency from combat and invests it into fighter stats, skills, and progression.

## Non-negotiable development rules
- No placeholder code, placeholder sprites, TODO-only systems, or fake interactions in committed work.
- Finish and test each change before committing it. A commit should represent a complete, playable improvement.
- Inspect the existing implementation before changing it; keep changes focused and preserve working systems.
- The arena and visible combat are the primary experience. Menus must support the fighting rather than obscure it.
- Every fighter must be a real, distinct visual asset with a readable silhouette and completed animation states before being introduced as playable.
- Do not claim a deployment succeeded until the GitHub Pages workflow for the latest commit reports success.
- Keep this document updated when core mechanics, controls, progression, or project structure change.

## Core loop
1. Buy/unlock fighters.
2. Fighters spawn on the arena stage.
3. When at least two opposing fighters are present, they automatically engage.
4. Combat resolves through visible movement, attacks, hit reactions, knockback, health, and defeat states.
5. Award currency and progression rewards for completed fights.
6. Upgrade health, damage, defense, movement, attack speed, energy, and abilities.
7. Unlock stronger fighters, skills, stages, and higher progression tiers.

## Combat requirements
- Side-view 2D fighting-game presentation inspired by classic MUGEN-style fighters.
- Fighters have independent health and energy resources, facing direction, movement, attack states, hitstun, knockback, cooldowns, and defeat handling.
- Basic attacks and special moves must be represented by visible animations and effects, not just floating damage numbers.
- Abilities have readable startup, active, and recovery phases. Strong attacks should have distinctive effects and meaningful cooldowns/costs.
- Combat must remain deterministic and stable at different frame rates; use a fixed-step simulation or equivalent delta-time handling.
- Fighters must not attack when there is no valid opponent.
- Prevent overlapping fighters, stage exits, and attacks that hit through invalid range.
- Show health bars and clear combat feedback.

## Incremental systems
- Currency is earned through actual combat outcomes.
- Upgrades have visible prices, clear effects, and scaling costs.
- The player can inspect owned fighters and choose which fighter to upgrade.
- Save progression locally and handle offline/returning play fairly without allowing absurd negative or unbounded values.
- UI values must always reflect the actual simulation state.

## Platform and UX
- Build as a responsive browser game, with desktop as the primary development/test target and mobile layouts supported.
- Use readable typography, clear contrast, and large interactive controls.
- Keep the arena visible at common desktop and phone aspect ratios.
- Avoid excessive UI clutter and avoid tiny text.

## Art and IP policy
- Target the visual language of classic MUGEN fighting games: hand-authored 2D character sprites, crisp silhouettes, expressive poses, frame-based animation, bold hit effects, dramatic special moves, and stage depth.
- Create original fighters, stages, effects, and UI. Do not extract or redistribute copyrighted sprites, character art, music, or other assets from commercial games or fan projects unless the user supplies assets they have rights to use or the assets are explicitly licensed for this use.
- Dragon Ball-like energy, martial-arts spectacle, and shonen intensity may inform the broad genre feel, but characters and designs must be original rather than copied.
- See `ART_SOURCE.md` for detailed asset requirements.

## Initial milestone
A complete playable vertical slice with an arena, at least two original fighters, actual sprite animations, automatic combat, health bars, hit reactions, special attacks, currency rewards, and working upgrades. Do not call the milestone complete if any of these are mocked or nonfunctional.
