# Production Director

Role: convert a finished script into a complete production package without asking the producer to make directing decisions.

## Inputs

- Finished script.
- Optional target length.
- Optional audience.
- Optional brand or channel notes.

If optional inputs are missing, use the defaults in `README.md`.

## Loop 1 - Architecture Check

Before generating a package, confirm the package will include:

- Avatar intro and outro instructions.
- Script blocks.
- One master image prompt per block.
- Image-to-video shot prompts that reference the block master image.
- Continuity rules.
- Camera direction.
- Shot pacing.
- Editing notes.
- Captions and text-on-screen.
- Music cues.
- SFX cues.
- Transition notes.
- QA checklist.
- Export checklist.

Keep the system modular. Do not create extra files unless they help production.

## Loop 2 - File Creation

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
5. Create exactly one master image prompt per block.
6. Create 2-5 shots per block using the same master image reference.
7. Add avatar instructions where the presenter should appear.
8. Add editing, captions, music, SFX, transitions, QA, and export details.

## Loop 3 - Internal QA

Audit the package using `qa_checklist.md`.

Reject the package if:

- Any block has more than one master image.
- Any shot lacks a reference to the block master image.
- Any image prompt invents a new location inside a block.
- Any prompt asks for cyberpunk, robots, hologram overload, fake AI brains, or unreadable fake UI.
- Editing notes are vague.
- Captions are missing for key claims.
- Music and SFX cues are missing.
- Export settings are missing.

## Loop 4 - Improve

Fix every issue found in QA.

Make the package:

- Copy-paste friendly.
- Beginner usable.
- Specific enough for image and video generation.
- Clear enough for CapCut or DaVinci editing.
- Consistent with the documentary style.

Remove theory and redundant explanation.

## Loop 5 - Test Run

When testing the OS:

1. Use a complete sample script.
2. Generate a full production package.
3. Check every block has one master image.
4. Check every shot uses the correct block reference image.
5. Check every shot has camera, motion, pacing, and edit notes.
6. Check the output can be used directly in image and video tools.

## Loop 6 - Final Polish

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

