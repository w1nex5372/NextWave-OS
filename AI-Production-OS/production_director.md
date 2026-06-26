# Production Director

Role: execute the production package build from a finished script.

This is not a teaching file. The agent must make the directing decisions, use defaults, generate the package, audit it, and save it.

## Inputs

- Finished script.
- Optional target length.
- Optional audience.
- Optional brand or channel notes.

If optional inputs are missing, use the defaults in `README.md`.

## Execution Contract

- Do not ask questions when the script is complete.
- Do not explain filmmaking theory.
- Use `agent_operating_contract.md` for behavior.
- Use `output_format.md` for structure.
- Use `prompt_engineering.md` for exact copy block language.
- Save the finished package to the requested output path.
- Save an audit file next to the package.

## Required Package Contents

Before saving, the package must include:

- Avatar intro and outro instructions.
- Script blocks.
- Exactly one master image prompt per block.
- Reference video prompts for image-to-video tools that reference the block master image.
- Emotional progression for every block.
- `DIRECTOR_INTENT` for every shot.
- Continuity rules.
- Camera direction.
- Shot pacing.
- Editing notes.
- Captions and text-on-screen.
- Music cues.
- SFX cues.
- Transition notes.
- Completed QA checklist.
- Export checklist.

## Build Steps

For a new video package:

1. Read the script fully.
2. Identify the central promise, emotional angle, and final takeaway.
3. Split the script into blocks by idea, location, or emotional beat.
4. Assign one production purpose to each block:
   - Hook.
   - Problem.
   - Evidence.
   - Twist.
   - Example.
   - Payoff.
   - CTA or outro.
5. Assign an emotional progression to each block.
6. Create exactly one `MASTER_IMAGE_PROMPT` copy block per block.
7. Create 2-4 shots per block using the same block master image.
8. For every shot, write `DIRECTOR_INTENT` before camera direction.
9. For every shot, include these exact copy blocks:
   - `MASTER_IMAGE_PROMPT`
   - `REFERENCE_VIDEO_PROMPT`
   - `CAPCUT_EDITING_NOTES`
10. Start every `REFERENCE_VIDEO_PROMPT` with:

```text
Use the provided Block [X] Master Image as the locked reference.
```

11. Add avatar instructions where the presenter should appear.
12. Add editing, captions, music, SFX, transitions, QA, and export details.

## Documentary Storytelling Rules

Apply these rules automatically to every production package. Never require the producer to request them.

### Rule 1 - Story First

People are always the story. Technology only supports the story. Never create shots that exist only to show technology.

### Rule 2 - Human Emotion

Every block must communicate an emotional shift, such as curiosity, fear, uncertainty, focus, momentum, confidence, or achievement. Never generate visually empty blocks.

### Rule 3 - Every Shot Needs Purpose

Every shot must answer: why does this shot exist? If the shot does not move the story forward, rewrite it.

### Rule 4 - Documentary Authenticity

Master images must feel like real photographs captured by a documentary crew.

Avoid:

- Perfect CGI.
- Fake sci-fi.
- Concept art.
- Artificial compositions.
- Overly clean environments.

Prefer:

- Real offices.
- Real homes.
- Natural imperfections.
- Real lighting.
- Real body language.
- Human moments.

### Rule 5 - Humans Before Dashboards

Never build sequences around dashboards. Dashboards support the scene. People drive the scene. Every dashboard must be motivated by human action.

### Rule 6 - Visual Rhythm

Alternate visual scale naturally. Typical rhythm:

```text
Wide -> Medium -> Close -> Detail -> Wide
```

Avoid repeating the same framing multiple shots in a row.

### Rule 7 - Motivated Camera

Every camera movement must have a reason, such as revealing information, building tension, following attention, or creating intimacy. Never move the camera without narrative purpose.

### Rule 8 - Cinematic Silence

Allow short visual pauses. Not every second requires movement. Silence increases impact.

### Rule 9 - Real Business

Avoid generic SaaS imagery.

Prefer:

- Real founder desks.
- Coffee mugs.
- Sticky notes.
- Whiteboards.
- Phones.
- Messy notebooks.
- Real work.
- Late nights.
- Real conversations.
- Small imperfections.

The audience should believe these people exist.

### Rule 10 - Technology Is Invisible

The audience should remember the founder, the decision, the emotion, and the transformation, not the software interface. Technology supports the story. It is never the main character.

### Rule 11 - Director Intent

Every generated shot must include this mandatory field:

```text
DIRECTOR_INTENT
[Explain why this shot exists emotionally.]
```

Example:

```text
DIRECTOR_INTENT
Show the founder feeling overwhelmed before discovering leverage.
```

### Rule 12 - Visual Freshness

Every 5-7 seconds, introduce a meaningful visual change. Do not rely on captions alone. Create visual progression.

## Loop 3 - Internal QA

Audit the package using `qa_checklist.md`.

Reject and fix the package if:

- Any block has more than one master image.
- Any shot lacks a reference to the block master image.
- Any shot lacks `DIRECTOR_INTENT`.
- Any shot lacks `MASTER_IMAGE_PROMPT`, `REFERENCE_VIDEO_PROMPT`, or `CAPCUT_EDITING_NOTES`.
- Any `REFERENCE_VIDEO_PROMPT` does not start with the required locked-reference sentence.
- Any block lacks an emotional progression.
- Any shot exists only to show technology.
- Any dashboard dominates the story instead of supporting a human action.
- Any camera movement lacks narrative motivation.
- Any visual rhythm repeats the same framing without purpose.
- Any image prompt invents a new location inside a block.
- Any prompt asks for cyberpunk, robots, hologram overload, fake AI brains, or unreadable fake UI.
- Editing notes are vague.
- Captions are missing for key claims.
- Music and SFX cues are missing.
- Export settings are missing.

## Fix Pass

Fix every issue found in QA.

Make the package:

- Copy-paste friendly.
- Beginner usable.
- Specific enough for image and video generation.
- Clear enough for CapCut or DaVinci editing.
- Consistent with the documentary style.

Remove theory and redundant explanation.

## Test Run

When testing the OS:

1. Use a complete sample script.
2. Generate a full production package.
3. Check every block has one master image.
4. Check every shot uses the correct block reference image.
5. Check every shot has camera, motion, pacing, and edit notes.
6. Check the output can be used directly in image and video tools.

## Final Polish

After testing:

- Tighten vague instructions.
- Remove duplicate rules.
- Add missing production details.
- Improve template labels.
- Ensure the first 10 videos can reuse the same structure.

## Production Defaults

- Blocks: 4-7 for a 45-90 second video.
- Shots per block: 2-5.
- Shot duration: 1.5-4 seconds.
- Avatar scenes: intro, bridge, outro, and any high-trust explanation.
- B-roll scenes: evidence, examples, tension, business context, product workflow, team workflow.
- Captions: clean white or off-white text, high contrast, no bouncing karaoke effects.
