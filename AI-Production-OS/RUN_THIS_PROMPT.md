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

Input script:
- AI-Production-OS/scripts/video_01_script.md

Output file:
- AI-Production-OS/output/production_package_video_01_v2.md

Audit file:
- AI-Production-OS/output/test_audit_video_01_v2.md

Task:
Turn the input script into a complete production-ready package for a vertical short-form AI business documentary.

Hard rules:
- Do not ask the producer questions.
- Use default assumptions when details are missing.
- Enforce One Block = One Master Image.
- Every block must have exactly one MASTER_IMAGE_PROMPT copy block.
- Every block must include an emotional progression.
- Every shot must include DIRECTOR_INTENT.
- Every shot must use the provided Block [X] Master Image as the locked reference.
- Every shot must include these copy blocks:
  - MASTER_IMAGE_PROMPT
  - REFERENCE_VIDEO_PROMPT
  - CAPCUT_EDITING_NOTES
- Every REFERENCE_VIDEO_PROMPT must start with:
  "Use the provided Block [X] Master Image as the locked reference..."
- Avoid cyberpunk, random robots, fake AI brains, excessive holograms, unreadable fake UI, glitch effects, and cheap TikTok effects.
- Save the finished production package to the output file.
- Save the audit checklist to the audit file.
```
