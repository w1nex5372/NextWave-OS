# AI Production OS

Purpose: turn any finished short-form documentary script into a production-ready package for avatar recording, image generation, image-to-video generation, and editing.

This OS is built for premium AI/business documentary videos with realistic corporate visuals. It makes directing decisions automatically so the producer can paste a script and receive copy-ready prompts, shot instructions, editing notes, captions, music cues, SFX cues, QA checks, and export checks.

## Core Rule

One Block = One Master Image.

Every shot in a block must use that block's master image as the visual reference. Do not create a new environment inside a block unless the story clearly changes location.

## Folder Map

- `production_director.md`: step-by-step operating loop for converting a script into a production package.
- `agent_operating_contract.md`: strict agent behavior, defaults, failure rules, and execution order.
- `RUN_THIS_PROMPT.md`: exact producer prompt to paste into Claude Code.
- `documentary_style.md`: visual identity, allowed looks, banned looks, and environment rules.
- `continuity_rules.md`: strict rules for reference images, character consistency, props, screen content, and locations.
- `cinematography.md`: camera language, shot types, movement, lens feel, lighting, and pacing defaults.
- `editing.md`: edit rhythm, transitions, captions, sound, music, and export guidance.
- `prompt_engineering.md`: copy-ready formulas for master image prompts and image-to-video prompts.
- `retention_rules.md`: short-form hook, structure, pacing, curiosity, and viewer retention rules.
- `output_format.md`: required final package structure.
- `qa_checklist.md`: audit checklist for the OS and generated production packages.
- `templates/`: reusable templates for videos, blocks, shots, and final packages.
- `scripts/`: input scripts.
- `examples/`: worked examples and producer-facing references.
- `output/`: generated production packages.

## 5-Step Beginner Workflow

1. Put the finished script in `scripts/video_XX_script.md`.
2. Open `RUN_THIS_PROMPT.md`.
3. Copy the full prompt and paste it into Claude Code.
4. Change the input and output filenames if needed.
5. Use the generated package from `output/` to create avatar scenes, master images, reference videos, captions, music, SFX, and the final edit.

## Single Producer Command

Use [RUN_THIS_PROMPT.md](RUN_THIS_PROMPT.md). It contains the exact copy-paste prompt for Claude Code.

## Default Production Assumptions

- Format: vertical 9:16 short-form documentary.
- Length: 45-90 seconds unless the script requires otherwise.
- Avatar: realistic presenter, clean studio or premium office background.
- Visual style: Netflix business documentary meets Apple, Google, and Microsoft corporate realism.
- Edit style: fast but premium, no cheap effects.
- Tools: HeyGen, Midjourney, ChatGPT image generation, Runway, Kling, Hailuo, Pika, Minimax, CapCut, DaVinci Resolve.
