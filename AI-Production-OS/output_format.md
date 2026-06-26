# Output Format

Every production package must follow this structure exactly.

Use fenced copy blocks. Labels must match exactly.

## 1. Production Summary

- Video title:
- Target length:
- Format:
- Core promise:
- Viewer takeaway:
- Visual style:
- Tool targets:

## 2. Avatar Intro

- Placement:
- Background:
- Wardrobe:
- Performance:
- Exact script lines:
- HeyGen notes:

## 3. Block Plan And Shot List

For each block:

- Block number:
- Block purpose:
- Emotional progression:
- Script lines:
- Location:
- Visual continuity summary:
- Master image prompt:
- Shots:

Each block must include exactly one block-level copy block:

```text
MASTER_IMAGE_PROMPT
[copy-ready image generation prompt]
```

Each shot inside the block must include:

- Shot ID:
- Timing:
- Voiceover/script line:
- DIRECTOR_INTENT:
- Reference image:
- Camera direction:
- Caption/text-on-screen:
- Music:
- SFX:
- Transition:
- Editor note:

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

- Placement:
- Background:
- Wardrobe:
- Performance:
- Exact script lines:
- HeyGen notes:

## 5. Continuity Rules For This Video

- Locked avatar identity:
- Locked environments:
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

## 7. QA Checklist

Include pass/fail checks from `qa_checklist.md`.

## 8. Export Checklist

Include final export settings and platform safety checks.
