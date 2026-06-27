# Prompt Engineering

All prompts must be copy-ready.

## Master Image Prompt Formula

Target 200-300 words. The prompt body has a hard maximum of 300 words, excluding the `MASTER_IMAGE_PROMPT` label.

Prioritize:

1. Location and architecture.
2. People and wardrobe.
3. Lighting and mood.
4. Continuity lock.
5. Negative prompt.

Do not overload the master prompt with per-shot actions, camera choreography, editing direction, or repeated style prose. Those details belong in the shot prompts.

Every master prompt belongs to exactly one script block. Never reuse it across blocks.

Before writing the prompt, resolve:

- `SCENE_SOURCE` with exact script evidence.
- Explicit environment and characters.
- Prior block environment state.
- Current block environment state.
- Continuity carried forward.
- New elements introduced by this block.
- Future-story elements forbidden from this block.
- Founder posture and business maturity.

```text
Create a realistic cinematic vertical 9:16 documentary frame for a premium business documentary.
Script block: Block [X] only.
Scene source: [environment, characters, primary subject, secondary subject, narrative stage, exact script evidence].
Scene: [single environment state for this block].
Visual subject: [the world, environment, situation, and people described by the narration].
Subjects: [people or objects].
Action: [what is happening in the still frame].
Mood: [emotion and story function].
Visual style: Netflix business documentary, Apple/Google/Microsoft corporate realism, modern SaaS startup polish.
Camera: [shot size, lens feel, angle].
Lighting: [specific realistic lighting].
Details: [props, wardrobe, screen style, environment details].
Continuity carried forward: [identity, wardrobe, architecture, and previously established objects].
Current-block additions: [only elements introduced by Block X].
Future-story exclusions: [props, outcomes, maturity, and information from Blocks X+1 onward].
Continuity lock: this is the unique master reference owned by Block [X]. It must support every shot in Block [X] and must not be reused by another block.
Avoid: future-block elements, unexplained object removal, teleported props, cyberpunk, random robots, hologram overload, fake AI brain, unreadable fake text, glitch effects, sci-fi neon, distorted hands, distorted faces, extra fingers, warped screens, logos unless supplied.
```

Reject the prompt if its environment, characters, or visual subject cannot be traced directly to `SCENE_SOURCE`.

## Reference Video Prompt Formula

Every reference video prompt must be copy-ready for Hailuo, Kling, Runway, Pika, and Minimax.

The reference image must be the unique master image owned by the shot's script block. Never reference a master image from another block.

Every reference video prompt must start with this exact sentence:

```text
Use the provided Block [X] Master Image as the locked reference.
```

```text
Use the provided Block [X] Master Image as the locked reference. Preserve the same location, lighting, color palette, people, wardrobe, props, screen style, and time of day.
Action: [single action or visual change].
Camera: [one camera move only].
Duration: [seconds].
Motion: subtle realistic documentary motion.
Continuity: no scene change, no new environment, no new people, no wardrobe change, no screen redesign.
Avoid: morphing, distorted hands, extra fingers, warped faces, changing furniture, changing screen layout, unreadable text, cyberpunk, robots, holograms, glitch effects.
```

## Required Shot Copy Blocks

Every shot must include the complete cinematic decision header before these three copy blocks:

```text
SHOT_TYPE
[Choose from shot_language.md.]

DIRECTOR_INTENT
[Explain why this shot exists emotionally and how it moves the human story forward.]

LENS
[Choose from lens_language.md.]

CAMERA_MOVEMENT
[Choose from camera_language.md and state its motivation.]

COMPOSITION
[Choose from composition_language.md.]

LIGHTING
[Choose from lighting_language.md.]

COLOR_STATE
[Choose from color_script.md.]

B-ROLL_STRATEGY
[State whether the shot is primary action, reaction, insert, cutaway, or B-roll support.]

EDITOR_NOTES
[State how the shot functions in the sequence and edit.]
```

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

## Avatar Prompt Formula

Use this formula only when the locked script explicitly defines a presenter scene. Never generate an avatar prompt from narration alone.

A script-authorized Avatar Intro or Avatar Outro is mandatory and overrides documentary visualization rules.

```text
Avatar: realistic presenter, calm documentary authority, direct eye contact, restrained gestures.
Wardrobe: modern premium business casual.
Background: clean premium studio or modern office, softly lit, uncluttered.
Lighting: [motivated key, fill, practicals, background separation].
Lens: [lens choice].
Camera movement: [locked or one motivated move].
Camera framing: [shot size, height, eye line, head room].
Facial emotion: [specific restrained emotion].
Performance notes: [tone, script-defined pace, gesture limits].
HeyGen notes: [avatar settings, lip-sync, gesture, eye-line, render notes].
Script lines: [exact lines].
```

## Negative Prompt Block

Use this negative prompt for all image and video tools:

```text
cyberpunk, neon sci-fi, random robots, fake AI brain, excessive holograms, glitch effects, TikTok effects, unreadable text, gibberish UI, warped screens, distorted faces, distorted hands, extra fingers, duplicate people, melted objects, logo artifacts, oversaturated colors, cartoon style, anime style, plastic skin
```

## Prompt Quality Checklist

Every prompt must specify:

- Vertical 9:16.
- Realistic documentary style.
- `VISUAL_SUBJECT` represented as the visible documentary world.
- One environment.
- People or objects.
- Action.
- Camera.
- Lighting.
- Continuity lock.
- Avoid list.
