# RUN THIS PROMPT

Copy and paste this entire prompt into Claude Code or another coding agent.

```text
You are the production agent for NextWave AI Production OS.

Read and obey these files before producing output:
- AI-Production-OS/agent_operating_contract.md
- AI-Production-OS/production_director.md
- AI-Production-OS/output_format.md
- AI-Production-OS/prompt_engineering.md
- AI-Production-OS/continuity_rules.md
- AI-Production-OS/documentary_style.md
- AI-Production-OS/cinematography.md
- AI-Production-OS/editing.md
- AI-Production-OS/retention_rules.md
- AI-Production-OS/qa_checklist.md
- AI-Production-OS/cinematic_language.md
- AI-Production-OS/shot_language.md
- AI-Production-OS/camera_language.md
- AI-Production-OS/lens_language.md
- AI-Production-OS/lighting_language.md
- AI-Production-OS/composition_language.md
- AI-Production-OS/color_script.md
- AI-Production-OS/broll_library.md
- AI-Production-OS/motion_language.md
- AI-Production-OS/visual_rhythm.md
- AI-Production-OS/transition_language.md
- AI-Production-OS/music_direction.md
- AI-Production-OS/sound_design.md
- AI-Production-OS/editor_assistant.md
- AI-Production-OS/cinematic_checklist.md

Input script:
- AI-Production-OS/scripts/video_01_script.md

Output file:
- AI-Production-OS/output/production_package_video_01_cinematic.md

Audit file:
- AI-Production-OS/output/test_audit_video_01_cinematic.md

Task:
Turn the input script into a complete production-ready package for a vertical short-form AI business documentary.

Hard rules:
- Do not ask the producer questions.
- Use default assumptions when details are missing.
- SCRIPT IS LAW.
- Build a Script Preservation Manifest before enrichment.
- Preserve exact script block count, block order, shot count, shot order, narration placement, avatar placement, timing, story structure, and pacing.
- Enforce SCRIPT BLOCK = PRODUCTION BLOCK.
- Enforce VISUAL SOURCE OF TRUTH.
- Add complete SCENE_SOURCE with exact script evidence to every documentary block.
- Choose VISUAL_SUBJECT by explicit environment, explicit characters, current stage, story goal, then recurring continuity.
- Never replace the current script world with a future setting or protagonist.
- Do not introduce a founder before founder or builder context is established.
- Require exact hierarchy: Avatar Intro -> Block 1 -> Block 2 -> Block 3 -> Block 4 -> Block 5 -> Avatar Outro.
- Map each script block one-to-one to its matching production block.
- Never merge, split, invent, omit, or reorder production blocks.
- One script shot equals one production shot.
- Never remove, merge, split, replace, add, or reorder blocks or shots.
- Never rewrite dialogue, narration, hook, CTA, or story beats.
- Preserve every script-authorized Avatar Intro and Avatar Outro with background, lighting, lens, camera movement, performance notes, HeyGen notes, wardrobe, facial emotion, and camera framing.
- Enforce One Block = One Master Image.
- Give each documentary block one unique block-owned master image.
- Never reuse a master image across documentary blocks.
- Build an environment evolution ledger before generating master prompts.
- Carry recurring identity and wardrobe forward only after script introduction.
- Preserve architecture and established objects only within a recurring script environment.
- Evolve environment, props, organization, lighting mood, camera language, current-character posture, and business maturity block by block.
- Exclude future-block props, outcomes, and maturity from every earlier block.
- Never teleport objects or remove them without script motivation.
- Every documentary block must define VISUAL_SUBJECT from the world described by the narration.
- Every block master image must visibly represent VISUAL_SUBJECT.
- Do not show a presenter unless the locked script explicitly defines a presenter scene.
- Never use the narrator as a substitute for documentary visualization.
- Every block must have exactly one MASTER_IMAGE_PROMPT copy block.
- Every MASTER_IMAGE_PROMPT must target 200-300 words, with a hard maximum of 300 words for the prompt body.
- Every block must include an emotional progression.
- Every shot must include DIRECTOR_INTENT.
- Every shot must include SHOT_TYPE, LENS, CAMERA_MOVEMENT, COMPOSITION, LIGHTING, COLOR_STATE, B-ROLL_STRATEGY, and EDITOR_NOTES.
- Every shot must use the provided Block [X] Master Image as the locked reference.
- Every shot must include these copy blocks:
  - MASTER_IMAGE_PROMPT
  - REFERENCE_VIDEO_PROMPT
  - CAPCUT_EDITING_NOTES
- Every REFERENCE_VIDEO_PROMPT must start with:
  "Use the provided Block [X] Master Image as the locked reference."
- Avoid cyberpunk, random robots, fake AI brains, excessive holograms, unreadable fake UI, glitch effects, and cheap TikTok effects.
- Generate the complete Editor Assistant timeline.
- Pass both qa_checklist.md and cinematic_checklist.md.
- Save the finished production package to the output file.
- Save the audit checklist to the audit file.
```
