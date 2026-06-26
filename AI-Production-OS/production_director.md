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
5. Create exactly one `MASTER_IMAGE_PROMPT` copy block per block.
6. Create 2-4 shots per block using the same block master image.
7. For every shot, include these exact copy blocks:
   - `MASTER_IMAGE_PROMPT`
   - `REFERENCE_VIDEO_PROMPT`
   - `CAPCUT_EDITING_NOTES`
8. Start every `REFERENCE_VIDEO_PROMPT` with:

```text
Use the provided Block [X] Master Image as the locked reference.
```

9. Add avatar instructions where the presenter should appear.
10. Add editing, captions, music, SFX, transitions, QA, and export details.

## Loop 3 - Internal QA

Audit the package using `qa_checklist.md`.

Reject and fix the package if:

- Any block has more than one master image.
- Any shot lacks a reference to the block master image.
- Any shot lacks `MASTER_IMAGE_PROMPT`, `REFERENCE_VIDEO_PROMPT`, or `CAPCUT_EDITING_NOTES`.
- Any `REFERENCE_VIDEO_PROMPT` does not start with the required locked-reference sentence.
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
