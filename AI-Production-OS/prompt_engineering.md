# Prompt Engineering

All prompts must be copy-ready.

## Master Image Prompt Formula

```text
Create a realistic cinematic vertical 9:16 documentary frame for a premium business documentary.
Scene: [single environment for this block].
Subjects: [people or objects].
Action: [what is happening in the still frame].
Mood: [emotion and story function].
Visual style: Netflix business documentary, Apple/Google/Microsoft corporate realism, modern SaaS startup polish.
Camera: [shot size, lens feel, angle].
Lighting: [specific realistic lighting].
Details: [props, wardrobe, screen style, environment details].
Continuity lock: this image is the master reference for Block [number]. It must support multiple shots in the same location.
Avoid: cyberpunk, random robots, hologram overload, fake AI brain, unreadable fake text, glitch effects, sci-fi neon, distorted hands, distorted faces, extra fingers, warped screens, logos unless supplied.
```

## Reference Video Prompt Formula

Every reference video prompt must be copy-ready for Hailuo, Kling, Runway, Pika, and Minimax.

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

Every shot must include these three copy blocks:

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

```text
Avatar: realistic presenter, calm documentary authority, direct eye contact, restrained gestures.
Wardrobe: modern premium business casual.
Background: clean premium studio or modern office, softly lit, uncluttered.
Performance: [tone], [pace], [emotion].
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
- One environment.
- People or objects.
- Action.
- Camera.
- Lighting.
- Continuity lock.
- Avoid list.
