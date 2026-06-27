# Production Package Template

## SCRIPT IS LAW

### Script Preservation Manifest

- Source script:
- Source documentary block count:
- Package documentary block count:
- Source shot count:
- Package shot count:
- Block order match: PASS/FAIL
- Shot order match: PASS/FAIL
- Narration match: PASS/FAIL
- Timing and pacing match: PASS/FAIL
- Avatar placement match: PASS/FAIL
- Preservation result: PASS/FAIL

One script shot equals one production shot. Do not remove, merge, split, replace, add, or reorder any script block or shot.

One script block equals one production block. Required hierarchy:

```text
Avatar Intro
-> Block 1
-> Block 2
-> Block 3
-> Block 4
-> Block 5
-> Avatar Outro
```

## 1. Production Summary

- Video title:
- Target length:
- Format: vertical 9:16
- Core promise:
- Viewer takeaway:
- Visual style: premium business documentary, realistic corporate visuals
- Tool targets: HeyGen, image generation, Hailuo/Kling/Runway/Pika/Minimax, CapCut/DaVinci

## 2. Avatar Intro

This script-defined section is mandatory and may not be marked `Not used`.

- Script authorization:
- Script shot count:
- Script shot IDs:
- Timing:
- Placement:
- Background:
- Lighting:
- Lens:
- Camera movement:
- Wardrobe:
- Facial emotion:
- Camera framing:
- Performance notes:
- Exact script lines:
- HeyGen notes:

Repeat this complete field set once per script-authorized Avatar Intro shot.

## 3. Block Plan And Shot List

Render the complete block schema exactly five times in source order:

```text
Block 1 -> Master Image 1 -> Block 1 Shots
Block 2 -> Master Image 2 -> Block 2 Shots
Block 3 -> Master Image 3 -> Block 3 Shots
Block 4 -> Master Image 4 -> Block 4 Shots
Block 5 -> Master Image 5 -> Block 5 Shots
```

Never reuse a master image across blocks.

### Block [Number] - [Purpose]

- Block number:
- Script block ID:
- Script block order:
- Script shot count:
- SCENE_SOURCE:
  - Environment:
  - Characters:
  - Primary Subject:
  - Secondary Subject:
  - Narrative Stage:
  - Evidence From Script:
- Prior block environment state:
- Current block environment state:
- Continuity carried forward:
- New elements introduced in this block:
- Future-story elements forbidden in this block:
- Founder posture:
- Business maturity state:
- Block purpose:
- Emotional progression:
- Color progression:
- Visual rhythm plan:
- Script lines:
- VISUAL_SUBJECT:
- Location:
- Visual continuity summary:
- Master image prompt: exactly one Block [Number] master image
- Shots:

#### Master Image Prompt

Target 200-300 words. The prompt body has a hard maximum of 300 words.

```text
MASTER_IMAGE_PROMPT
[Unique Block X prompt that represents only this script block, carries established continuity, adds current-block elements, and excludes future-block information.]
```

#### Shots

##### Shot [Number].[Number]

- Script shot ID:
- Script shot order:
- Timing:
- Voiceover/script line: [exact script text]
- SHOT_TYPE:
- DIRECTOR_INTENT:
- LENS:
- CAMERA_MOVEMENT:
- COMPOSITION:
- LIGHTING:
- COLOR_STATE:
- B-ROLL_STRATEGY:
- Reference image: Block [Number] unique master image only.
- Camera direction:
- Caption/text-on-screen:
- Music:
- SFX:
- Transition:
- Editor note:
- EDITOR_NOTES:

```text
MASTER_IMAGE_PROMPT
Use Block [Number] MASTER_IMAGE_PROMPT above. Do not create a new master image for this shot.
```

```text
REFERENCE_VIDEO_PROMPT
Use the provided Block [Number] Master Image as the locked reference. Preserve the same location, lighting, color palette, people, wardrobe, props, screen style, and time of day.
Action:
Camera:
Duration:
Motion: subtle realistic documentary motion.
Continuity: no scene change, no new environment, no new people, no wardrobe change, no screen redesign.
Avoid: morphing, distorted hands, extra fingers, warped faces, changing furniture, changing screen layout, unreadable text, cyberpunk, robots, holograms, glitch effects.
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

## 4. Avatar Outro

This script-defined section is mandatory and may not be marked `Not used`.

- Script authorization:
- Script shot count:
- Script shot IDs:
- Timing:
- Placement:
- Background:
- Lighting:
- Lens:
- Camera movement:
- Wardrobe:
- Facial emotion:
- Camera framing:
- Performance notes:
- Exact script lines:
- HeyGen notes:

Repeat this complete field set once per script-authorized Avatar Outro shot.

## 5. Continuity Rules For This Video

- Locked avatar identity:
- Locked recurring character identities:
- Locked recurring character wardrobe:
- Locked environments:
- Block 1 environment state:
- Block 2 environment evolution:
- Block 3 environment evolution:
- Block 4 environment evolution:
- Block 5 environment evolution:
- Object accumulation ledger:
- Future-information exclusions by block:
- Block-level reference rules:
- Prop rules:
- Screen rules:
- Color rules:

## 6. Editing Plan

- Timeline rhythm:
- Caption style:
- Transition style:
- Music arc:
- SFX approach:
- Color grade:

## 6A. Editor Assistant Timeline

### Track Layout

- V1:
- V2:
- V3:
- V4:
- A1:
- A2:
- A3:
- A4:
- A5:

### Time-Coded Timeline

| Time | Block | Shot ID | Master Reference | Video Track | Dialogue | Music | SFX | Subtitle | Transition | Speed | Color | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|

### CapCut Implementation Notes

- Music timing:
- SFX timing:
- Subtitle timing:
- Speed ramps:
- Zooms/reframes:
- J-cuts/L-cuts:
- Hold frames:
- Color grade notes:
- Export settings:

## 7. QA Checklist

- [ ] Script and package block counts match exactly.
- [ ] Hierarchy is Avatar Intro, Blocks 1-5, Avatar Outro.
- [ ] Every script block maps to one production block.
- [ ] Every documentary block includes `SCENE_SOURCE` with exact evidence from its script block.
- [ ] Every `VISUAL_SUBJECT`, environment, character, and primary subject is script-grounded.
- [ ] No founder appears before founder or builder context is established.
- [ ] No block is merged, split, invented, omitted, or reordered.
- [ ] Script and package shot counts match exactly.
- [ ] Every script shot maps to one production shot in source order.
- [ ] Narration, dialogue, hook, CTA, timing, pacing, story structure, and avatar placement are unchanged.
- [ ] Every script-authorized Avatar Intro and Avatar Outro is present with all required production fields.
- [ ] Every block has exactly one master image.
- [ ] Every block master image is unique and is never reused by another block.
- [ ] Every block excludes future-story props, outcomes, and maturity.
- [ ] Environment, props, organization, lighting mood, current-character posture, and business maturity evolve across Blocks 1-5.
- [ ] Recurring identity and script-defined wardrobe remain continuous after introduction.
- [ ] Objects accumulate naturally without teleporting or disappearing.
- [ ] Every master image prompt targets 200-300 words, and its prompt body does not exceed 300 words.
- [ ] Every documentary block has `VISUAL_SUBJECT`, and its master image represents it.
- [ ] No presenter appears in a documentary block without explicit script permission.
- [ ] Narration is visualized through its described world, people, actions, and consequences.
- [ ] Every shot uses its block master image as reference.
- [ ] Every shot includes all cinematic decision fields.
- [ ] No block changes location.
- [ ] All prompts avoid banned visuals.
- [ ] Editing notes are clear.
- [ ] Editor Assistant timeline is complete.
- [ ] `cinematic_checklist.md` passes.
- [ ] Export settings are complete.

## 8. Export Checklist

- [ ] 9:16 vertical.
- [ ] 1080x1920 or 2160x3840.
- [ ] Captions inside safe zones.
- [ ] Dialogue clean and audible.
- [ ] Music mixed below voice.
- [ ] First frame clear.
- [ ] Final file reviewed on mobile.
