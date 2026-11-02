# Idle Anime Fighters — Art Source Guide

## Visual target
A high-energy, classic 2D anime fighting-game look strongly informed by the presentation of MUGEN fighter games. The desired feel is closer to a hand-animated arcade fighter than a generic idle game: expressive sprite poses, readable silhouettes, dramatic hit-stop, impact flashes, knockback, energy effects, and richly illustrated stages.

## Originality and asset sourcing
- Prefer original, purpose-made assets created for this project.
- Do not rip, scrape, or redistribute sprites from MUGEN games, Dragon Ball games, anime, or other copyrighted works without permission or a license that allows this use.
- User-provided assets may be incorporated when the user has the rights to use and redistribute them.
- For third-party assets, record creator, source URL, license, attribution requirements, and any modification in an asset credits file.
- Do not use generated sprite sheets as final assets unless every frame is coherent, cleanly separated, correctly aligned, and manually checked at native scale.

## Character sprite requirements
- Characters are original anime martial artists with distinct proportions, costumes, hair silhouettes, palettes, and combat identities.
- Use sprite sheets or frame sequences with consistent frame dimensions, transparent backgrounds, stable feet baselines, and clear frame naming.
- Include, as appropriate: idle, walk, run/dash, jump, crouch, light attack, heavy attack, special attack, hurt, knockback, block, victory, and defeat.
- Animation frames must preserve character scale, anatomy, costume details, and facing direction.
- Provide left- and right-facing versions by authored frames or reliable sprite flipping; verify asymmetric details before flipping.
- Keep silhouettes readable against every stage background.
- No emoji, colored rectangles, stick figures, or generic icons in place of fighter sprites.

## Combat VFX
- Make hits feel forceful through layered impact bursts, slash arcs, speed lines, dust puffs, hit sparks, brief hit-stop, camera shake, and controlled screen flashes.
- Energy attacks need distinct authored projectile/beam visuals, charging cues, travel behavior, impact effects, and cooldown feedback.
- Effects must communicate attack strength and direction without obscuring the fighters for long periods.
- Use a consistent visual language for light, medium, heavy, and ultimate attacks.

## Stage art
- Side-view fighting stages with a clear floor plane and enough horizontal room for spacing, dashes, and knockback.
- Build depth with a foreground fighting plane, midground architecture/terrain, and distant scenery.
- Stage palettes should contrast with fighter palettes and effects.
- Include subtle environmental motion only where it adds atmosphere and does not distract from combat.

## UI art
- UI should feel like an arcade fighting game: compact status panels, sharp borders, restrained metallic or energy accents, clear labels, and bold readable numbers.
- Health and energy bars must be legible during action.
- Buttons and panels must remain usable on desktop and touch screens.
- The arena should occupy the largest share of the play screen.

## Quality gate before commit
- Inspect every sprite at native resolution and at intended in-game scale.
- Check frame alignment, transparency, silhouette readability, animation continuity, and facing direction.
- Check effects against light and dark stage areas.
- Confirm all referenced assets exist and load; no broken paths or missing frames.
- Play through the relevant combat states and verify that animation transitions do not pop, freeze, or show incorrect frames.
- Only commit finished, integrated assets and working code. No placeholder art or unfinished sprite sheets.
