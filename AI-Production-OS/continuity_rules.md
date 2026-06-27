# Continuity Rules

The OS must enforce continuity automatically.

Lens, movement, composition, lighting, and color may vary inside a block only when the master image can support the variation without changing the locked environment, people, wardrobe, props, time of day, or documentary realism.

## Non-Negotiable Rule

One Block = One Master Image.

SCRIPT BLOCK = PRODUCTION BLOCK.

Each of Blocks 1-5 owns one unique master image. Never reuse a master image across blocks and never create more than one master image inside a block.

Every shot in the same block must say:

```text
REFERENCE_VIDEO_PROMPT
Use the provided Block [X] Master Image as the locked reference. Preserve the same location, lighting, color palette, people, wardrobe, props, screen style, and time of day.
```

Every shot must also include:

```text
MASTER_IMAGE_PROMPT
Use Block [X] MASTER_IMAGE_PROMPT above. Do not create a new master image for this shot.
```

```text
CAPCUT_EDITING_NOTES
Timing:
Caption:
Music:
SFX:
Transition:
Editor note:
```

## Block Continuity

Inside one block:

- Do not change location.
- Do not change time of day.
- Do not change wardrobe.
- Do not introduce new hero props.
- Do not change screen design language.
- Do not change the number of main people unless the shot is a crop or angle change.
- Do not move from office to data center, studio, city street, or home unless a new block starts.

## Cross-Block Evolution

Across Blocks 1-5:

- Determine environment and characters from each block's `SCENE_SOURCE`.
- Lock a recurring character's identity, face, body proportions, hair, and script-defined wardrobe only after introduction.
- Do not force a future recurring founder into earlier worker, customer, city, factory, or corporate blocks.
- Preserve architectural identity only when the script remains in the same environment.
- Let the environment evolve only through additions and changes supported by the current script block.
- Carry established props forward when the narrative remains in the same environment; do not transplant props across unrelated locations.
- Introduce each new prop in the first block where it becomes narratively relevant.
- Never show future-block props, outcomes, organization, revenue signals, or business maturity early.
- Evolve lighting gradually with emotional progression; do not jump between unrelated times of day without script direction.
- Evolve current-character posture with the script. Apply founder posture continuity only after founder introduction.
- Keep an object accumulation ledger for every block.

Required progression check:

| Block | Chapter State | Environment Requirement |
|---|---|---|
| Block 1 | Fear / setup | Current problem world: corporate office, workers, headline pressure, and reactions when supported by script |
| Block 2 | Thinking | Script-supported individual or builder context; planning elements may begin |
| Block 3 | Building | Script-supported founder and build environment; connections or workflow evidence may appear |
| Block 4 | Operations | Founder operating with only script-supported active tasks and systems |
| Block 5 | Momentum | Script-supported leverage, mature organization, orders, or payoff |

This table defines progression logic, not permission to add an object absent from the script.

## Allowed Shot Variation Inside A Block

Allowed:

- Push-in.
- Pull-back.
- Pan.
- Tilt.
- Rack focus.
- Detail closeup.
- Over-the-shoulder angle.
- Wider angle of the same room.
- Cropped insert of the same props.
- Slow handheld documentary movement.

Not allowed:

- New room.
- New city.
- New team.
- New device style.
- New lighting scheme.
- New visual metaphor.

## Avatar Continuity

Apply these rules only to presenter scenes explicitly defined by the locked script. Narration alone does not authorize an avatar scene.

For authorized avatar scenes:

- Use the same presenter identity across intro and outro.
- Keep wardrobe consistent unless the producer specifies multiple episodes.
- Use a premium clean studio, modern office, or editorial background.
- Avatar should speak directly to camera with calm documentary authority.
- Avoid exaggerated gestures.

Do not carry the avatar into documentary blocks. Documentary blocks preserve their own `VISUAL_SUBJECT`, people, environment, and action independently of the narrator.

## Multi-Video Continuity

For the first 10 videos:

- Keep the avatar identity consistent.
- Keep title card style consistent.
- Reuse 3-5 environment families:
  - Premium office.
  - Founder workspace.
  - Product dashboard room.
  - Investor boardroom.
  - Customer operations floor.
- Keep caption style consistent.
- Keep music identity consistent.
