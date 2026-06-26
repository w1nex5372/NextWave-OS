# AI Production OS

Purpose: turn any finished short-form documentary script into a production-ready package for avatar recording, image generation, image-to-video generation, and editing.

This OS is built for premium AI/business documentary videos with realistic corporate visuals. It makes directing decisions automatically so the producer can paste a script and receive copy-ready prompts, shot instructions, editing notes, captions, music cues, SFX cues, QA checks, and export checks.

## Core Rule

One Block = One Master Image.

Every shot in a block must use that block's master image as the visual reference. Do not create a new environment inside a block unless the story clearly changes location.

## Folder Map

- `production_director.md`: step-by-step operating loop for converting a script into a production package.
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

## Standard Workflow

1. Paste a finished script into `scripts/video_XX_script.md`.
2. Ask the coding agent to run `production_director.md`.
3. The agent splits the script into blocks.
4. The agent creates exactly one master image prompt per block.
5. The agent creates all shot prompts using that block's master image as reference.
6. The agent adds avatar instructions, editing notes, captions, music, SFX, transitions, QA, and export checklist.
7. The agent audits the package against `qa_checklist.md`.

## Producer Prompt

```text
Use AI-Production-OS/production_director.md.
Turn scripts/video_XX_script.md into output/production_package_video_XX.md.
Enforce One Block = One Master Image.
Make the output copy-paste ready for HeyGen, image generation, image-to-video, and editing.
```

## Default Production Assumptions

- Format: vertical 9:16 short-form documentary.
- Length: 45-90 seconds unless the script requires otherwise.
- Avatar: realistic presenter, clean studio or premium office background.
- Visual style: Netflix business documentary meets Apple, Google, and Microsoft corporate realism.
- Edit style: fast but premium, no cheap effects.
- Tools: HeyGen, Midjourney, ChatGPT image generation, Runway, Kling, Hailuo, Pika, Minimax, CapCut, DaVinci Resolve.

