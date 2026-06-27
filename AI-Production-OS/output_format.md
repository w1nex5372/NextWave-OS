# Output Format

Every production package must follow this structure exactly.

Use fenced copy blocks. Labels must match exactly.

Compatibility: existing production packages remain valid historical artifacts. Every newly generated package must use the extended cinematic fields below.

## SCRIPT IS LAW

Every new package must begin with a Script Preservation Manifest:

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

The package may proceed only when every result is `PASS`. One script shot must map to exactly one production shot. Do not remove, merge, split, replace, add, or reorder blocks or shots.

Manifest block counts refer to documentary blocks. Avatar Intro and Avatar Outro are tracked separately through avatar placement.

The source and package documentary block counts must both equal `5`.

## 1. Production Summary

- Video title:
- Target length:
- Format:
- Core promise:
- Viewer takeaway:
- Visual style:
- Tool targets:

## 2. Avatar Intro

This script-defined section is mandatory. It may not be omitted, replaced, or marked `Not used`.

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

If Avatar Intro contains multiple script shots, repeat the complete avatar field set once per source shot in source order.

## 3. Block Plan And Shot List

Render five complete production blocks in this exact hierarchy:

```text
### Block 1
#### Master Image Prompt
#### Shots

### Block 2
#### Master Image Prompt
#### Shots

### Block 3
#### Master Image Prompt
#### Shots

### Block 4
#### Master Image Prompt
#### Shots

### Block 5
#### Master Image Prompt
#### Shots
```

Never merge, split, invent, omit, or reorder these blocks.

For each block:

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
- Master image prompt:
- Shots:

`SCENE_SOURCE` is mandatory and must cite exact lines from the current script block.

`VISUAL_SUBJECT` defines the documentary world. It must follow this priority: explicit environment, explicit characters, current narrative stage, story goal, recurring character continuity. The block master image must visibly represent it. Never replace the script world with a future setting or character.

Each block must include exactly one block-level copy block:

The `MASTER_IMAGE_PROMPT` must target 200-300 words. Its prompt body has a hard maximum of 300 words, excluding the `MASTER_IMAGE_PROMPT` label. Prioritize location, architecture, people, wardrobe, lighting, mood, continuity lock, and negative prompt. Put detailed shot action and movement in shot prompts.

Each block master image is unique to that block. It must carry established identity and continuity forward, add only current-block elements, explicitly exclude future-block elements, and never be reused by another block.

```text
MASTER_IMAGE_PROMPT
[copy-ready image generation prompt]
```

Each shot inside the block must include:

- Shot ID:
- Script shot ID:
- Script shot order:
- Timing:
- Voiceover/script line: exact script text
- SHOT_TYPE:
- DIRECTOR_INTENT:
- LENS:
- CAMERA_MOVEMENT:
- COMPOSITION:
- LIGHTING:
- COLOR_STATE:
- B-ROLL_STRATEGY:
- Reference image:
- Camera direction:
- Caption/text-on-screen:
- Music:
- SFX:
- Transition:
- Editor note:
- EDITOR_NOTES:

Each shot must include these exact copy blocks:

```text
MASTER_IMAGE_PROMPT
Use Block [X] MASTER_IMAGE_PROMPT above. Do not create a new master image for this shot.
```

```text
REFERENCE_VIDEO_PROMPT
Use the provided Block [X] Master Image as the locked reference. Preserve the same location, lighting, color palette, people, wardrobe, props, screen style, and time of day.
Action: [single action].
Camera: [one camera move only].
Duration: [seconds].
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

This script-defined section is mandatory. It may not be omitted, replaced, or marked `Not used`.

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

If Avatar Outro contains multiple script shots, repeat the complete avatar field set once per source shot in source order.

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

Include:

- Track layout.
- Complete time-coded shot table.
- Script block and unique block master reference for every documentary shot.
- Video track assignment.
- Dialogue track assignment.
- Music timing and drops.
- SFX timing.
- Subtitle timing.
- Speed ramps.
- Zooms or reframes.
- Transitions.
- J-cuts and L-cuts.
- Hold frames.
- Color grade notes.
- CapCut implementation notes.

## 7. QA Checklist

Include the `SCRIPT IS LAW` preservation checks plus pass/fail checks from `qa_checklist.md` and `cinematic_checklist.md`.

## 8. Export Checklist

Include final export settings and platform safety checks.
