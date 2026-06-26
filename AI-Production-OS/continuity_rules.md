# Continuity Rules

The OS must enforce continuity automatically.

## Non-Negotiable Rule

One Block = One Master Image.

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

For avatar scenes:

- Use the same presenter identity across intro and outro.
- Keep wardrobe consistent unless the producer specifies multiple episodes.
- Use a premium clean studio, modern office, or editorial background.
- Avatar should speak directly to camera with calm documentary authority.
- Avoid exaggerated gestures.

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
