# QA Checklist

Use this checklist before a production package is considered ready.

## OS QA

- [ ] A beginner can follow the workflow without filmmaking knowledge.
- [ ] The system turns a finished script into a complete production package.
- [ ] One Block = One Master Image is stated and enforced.
- [ ] Shot prompts require the block master image as reference.
- [ ] The style avoids random sci-fi visuals.
- [ ] Prompt formulas are copy-ready.
- [ ] Editing, music, SFX, captions, transitions, QA, and export guidance are included.
- [ ] Output format is strict.
- [ ] The structure supports at least the first 10 videos.
- [ ] Duplicate or confusing instructions are removed.

## Production Package QA

- [ ] Production summary is complete.
- [ ] Avatar intro instructions are complete.
- [ ] Avatar outro instructions are complete.
- [ ] Every block has exactly one master image prompt.
- [ ] Every shot references the correct block master image.
- [ ] Every shot includes `MASTER_IMAGE_PROMPT`, `REFERENCE_VIDEO_PROMPT`, and `CAPCUT_EDITING_NOTES` copy blocks.
- [ ] Every `REFERENCE_VIDEO_PROMPT` starts with "Use the provided Block [X] Master Image as the locked reference."
- [ ] No block changes location without starting a new block.
- [ ] Camera direction is specific for every shot.
- [ ] Shot timing is included.
- [ ] Captions or text-on-screen are included where needed.
- [ ] Music cues are included.
- [ ] SFX cues are included.
- [ ] Transitions are included.
- [ ] Negative prompts avoid cyberpunk, robots, fake AI brains, hologram overload, unreadable text, and cheap effects.
- [ ] Export checklist is complete.
