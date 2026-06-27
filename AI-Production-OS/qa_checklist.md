# QA Checklist

Use this checklist before a production package is considered ready.

## SCRIPT IS LAW

- [ ] A Script Preservation Manifest records source and package block counts, shot counts, order, narration placement, timing, pacing, and avatar placement.
- [ ] Manifest block counts match script-defined documentary blocks; avatar sections are tracked separately through avatar placement.
- [ ] Package block count exactly matches script block count.
- [ ] Package shot count exactly matches script shot count.
- [ ] Every script shot maps to exactly one production shot.
- [ ] No block or shot is removed, merged, split, replaced, added, or reordered.
- [ ] Exact narration, dialogue, hook, and CTA text is unchanged.
- [ ] Narration remains attached to its original block and shot.
- [ ] Story structure, production timing, and pacing match the script.
- [ ] Every script-authorized Avatar Intro and Avatar Outro remains in its original position.
- [ ] Every script avatar shot maps to exactly one production avatar shot with matching ID, order, timing, and exact lines.
- [ ] Documentary scenes and story beats are preserved, not replaced.

Any failed item rejects the package. Cinematic quality never overrides script authority.

## Script Block Architecture QA

- [ ] Hierarchy is exactly Avatar Intro, Block 1, Block 2, Block 3, Block 4, Block 5, Avatar Outro.
- [ ] Source and package documentary block counts both equal 5.
- [ ] Every production block maps one-to-one to the matching script block.
- [ ] No script blocks are merged.
- [ ] No script block is split.
- [ ] No production block is invented, omitted, or reordered.
- [ ] Every script shot remains inside its original script block.
- [ ] Every documentary block owns exactly one unique master image.
- [ ] No master image is reused across documentary blocks.
- [ ] Every shot references only its own block master image.
- [ ] Every block master image contains only current or previously established information.
- [ ] No block reveals future props, outcomes, business maturity, or story information.
- [ ] Environment, props, organization, lighting mood, camera language, current-character posture, and business maturity evolve with the story.
- [ ] Recurring character identity remains locked after script introduction.
- [ ] Recurring wardrobe remains locked unless the script explicitly changes it.
- [ ] Established objects carry forward or are removed only with visible script motivation.
- [ ] Objects never teleport, disappear without motivation, or appear before introduction.
- [ ] Emotional progression is visibly reflected in the environment.

Any failed item rejects the package.

## Visual Source Of Truth QA

- [ ] Every documentary block includes complete `SCENE_SOURCE`.
- [ ] Every `SCENE_SOURCE` cites exact evidence from its own script block.
- [ ] `VISUAL_SUBJECT` is directly supported by that evidence.
- [ ] Explicit script environment has priority over recurring character continuity.
- [ ] Explicit script characters have priority over future protagonist continuity.
- [ ] The environment matches the current narrative world.
- [ ] Characters appear only after the script establishes them.
- [ ] The founder does not appear before founder or individual-builder context.
- [ ] The solution does not appear before the problem is established.
- [ ] Future locations, props, outcomes, and business maturity remain excluded.
- [ ] A worker/headline/fear block visualizes workers, workplace pressure, headlines, and human reactions rather than a founder apartment.

Example rejection: script says `Every day people see the same headlines. AI is taking jobs.` but output shows a founder alone in an apartment.

## OS QA

- [ ] A beginner can follow the workflow without filmmaking knowledge.
- [ ] The system turns a finished script into a complete production package.
- [ ] One Block = One Master Image is stated and enforced.
- [ ] Shot prompts require the block master image as reference.
- [ ] The style avoids random sci-fi visuals.
- [ ] Prompt formulas are copy-ready.
- [ ] All cinematic language modules are referenced by the Production Director.
- [ ] Editing, music, SFX, captions, transitions, QA, and export guidance are included.
- [ ] Editor Assistant timeline guidance is included.
- [ ] Output format is strict.
- [ ] The structure supports at least the first 10 videos.
- [ ] Duplicate or confusing instructions are removed.

## Production Package QA

- [ ] Production summary is complete.
- [ ] Script-defined Avatar Intro is complete and is not marked `Not used`.
- [ ] Script-defined Avatar Outro is complete and is not marked `Not used`.
- [ ] Avatar Intro and Avatar Outro preserve their exact script positions and lines.
- [ ] Every authorized avatar shot includes background, lighting, lens, camera movement, performance notes, HeyGen notes, wardrobe, facial emotion, and camera framing.
- [ ] Every documentary block has exactly one unique block-owned master image prompt.
- [ ] Every master image prompt targets 200-300 words, and its prompt body does not exceed 300 words.
- [ ] Every documentary block has `VISUAL_SUBJECT`.
- [ ] Every master image visibly represents its block's `VISUAL_SUBJECT`.
- [ ] Every block contains an emotional progression.
- [ ] Every shot references the correct block master image.
- [ ] Every shot has `DIRECTOR_INTENT`.
- [ ] Every shot has `SHOT_TYPE`.
- [ ] Every shot has `LENS`.
- [ ] Every shot has `CAMERA_MOVEMENT`.
- [ ] Every shot has `COMPOSITION`.
- [ ] Every shot has `LIGHTING`.
- [ ] Every shot has `COLOR_STATE`.
- [ ] Every shot has `B-ROLL_STRATEGY`.
- [ ] Every shot has `EDITOR_NOTES`.
- [ ] Every shot includes `MASTER_IMAGE_PROMPT`, `REFERENCE_VIDEO_PROMPT`, and `CAPCUT_EDITING_NOTES` copy blocks.
- [ ] Every `REFERENCE_VIDEO_PROMPT` starts with "Use the provided Block [X] Master Image as the locked reference."
- [ ] Technology supports humans.
- [ ] No presenter appears in a documentary block without explicit script permission.
- [ ] The narrator never becomes the visual focus by default.
- [ ] Documentary blocks use cinematic visual storytelling rather than presenter coverage.
- [ ] The visuals represent the people, world, action, or consequence described by the narration.
- [ ] Dashboards never dominate the story.
- [ ] Camera movement has narrative motivation.
- [ ] Visual rhythm alternates naturally.
- [ ] The same lens, movement, framing, distance, or composition is not repeated more than twice without story justification.
- [ ] Color progression matches emotional progression.
- [ ] Music direction follows the story phases.
- [ ] Sound design is motivated and physically believable.
- [ ] Transition choices are motivated.
- [ ] The Editor Assistant timeline is complete and executable.
- [ ] Every rejection condition in `cinematic_checklist.md` passes.
- [ ] The production package feels like a Netflix documentary rather than an AI demo.
- [ ] No block changes location without starting a new block.
- [ ] Camera direction is specific for every shot.
- [ ] Shot timing is included.
- [ ] Captions or text-on-screen are included where needed.
- [ ] Music cues are included.
- [ ] SFX cues are included.
- [ ] Transitions are included.
- [ ] Negative prompts avoid cyberpunk, robots, fake AI brains, hologram overload, unreadable text, and cheap effects.
- [ ] Export checklist is complete.
