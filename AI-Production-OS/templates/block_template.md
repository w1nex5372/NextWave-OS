# Block Template

## SCRIPT IS LAW

This template expands one existing script block. It never creates, merges, splits, replaces, or moves a block.

This block owns exactly one unique master image. Its shots may not reference another block's master image.

## Block [Number]

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
- Purpose:
- Emotional progression:
- Color progression:
- Visual rhythm plan:
- Script lines:
- VISUAL_SUBJECT:
- Location:
- Emotional tone:
- Continuity summary:
- Primary shot type:
- Lens base:
- Camera movement strategy:
- Composition strategy:
- Lighting strategy:
- B-roll strategy:

## Master Image Prompt

Target 200-300 words. The prompt body has a hard maximum of 300 words. Prioritize location, architecture, people, wardrobe, lighting, mood, continuity lock, and negative prompt. Keep shot-specific action and movement in `shot_template.md`.

```text
MASTER_IMAGE_PROMPT
Create a realistic cinematic vertical 9:16 documentary frame for a premium business documentary.
Scene:
Visual subject: [Repeat this block's VISUAL_SUBJECT and make it the visible documentary world.]
Subjects:
Action:
Mood:
Visual style: Netflix business documentary, Apple/Google/Microsoft corporate realism, modern SaaS startup polish.
Shot type:
Lens:
Camera:
Composition:
Lighting:
Color state:
Details:
Continuity carried forward:
Current-block additions:
Future-story exclusions:
Continuity lock: this is the unique master reference owned by Block [number]. It must support every shot in this block and must not be reused by another block.
Avoid: future-block information, unexplained object removal, teleported props, cyberpunk, random robots, hologram overload, fake AI brain, unreadable fake text, glitch effects, sci-fi neon, distorted hands, distorted faces, extra fingers, warped screens, logos unless supplied.
```

## Shots

Use `shot_template.md` once for every script shot in this block. One script shot equals one production shot.
