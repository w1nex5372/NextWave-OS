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
- Use `cinematic_language.md` as the visual language bible.
- Use `shot_language.md`, `lens_language.md`, `camera_language.md`, `lighting_language.md`, and `composition_language.md` for shot design.
- Use `color_script.md`, `motion_language.md`, `visual_rhythm.md`, and `transition_language.md` for sequence design.
- Use `broll_library.md`, `music_direction.md`, `sound_design.md`, and `editor_assistant.md` for production execution.
- Use `cinematic_checklist.md` as the final cinematic rejection gate.
- Save the finished package to the requested output path.
- Save an audit file next to the package.

## SCRIPT IS LAW

The script is the highest authority. The production package may enrich the script, but it may never restructure, optimize, rewrite, shorten, expand, or reinterpret the script's production plan.

The script defines:

- Narration.
- Block order.
- Block count.
- Shot order.
- Shot count.
- Avatar placement.
- Production timing.
- Story structure.
- Pacing.

Before directing, create an internal one-to-one script manifest containing every script block, every script shot, exact narration, timing, and avatar placement in source order. The package must preserve that manifest exactly.

For manifest counts, `block count` means script-defined documentary blocks. Track Avatar Intro and Avatar Outro separately through avatar placement.

The Production Director may:

- Improve prompts.
- Improve cinematography and camera language.
- Improve documentary realism and continuity.
- Improve editing notes, sound design, and transitions.
- Improve emotional clarity and production quality without changing the story beat.

The Production Director must never:

- Remove, merge, split, replace, or reorder shots.
- Remove, merge, split, replace, or reorder blocks.
- Reduce or increase shot count.
- Invent a different visual structure.
- Move narration between shots or blocks.
- Change pacing, timing, or avatar placement.
- Rewrite dialogue, CTA, hooks, or narration.
- Replace documentary scenes or story beats.
- Optimize the script.

### Shot Preservation Rule

One script shot equals one production shot, including shots inside Avatar Intro and Avatar Outro.

If the script contains 28 shots, the package must contain 28 production shots in the same order. Expand each script shot with prompts, camera, lighting, sound, continuity, and editing direction. Never delete or combine it.

When a script uses explicit shot labels, preserve those IDs. When it uses discrete non-empty shot beats without numeric labels, preserve each beat as one shot in source order. Never consolidate beats for convenience.

### Block Preservation Rule

SCRIPT BLOCK = PRODUCTION BLOCK.

Use the script's explicit block boundaries and order. Every production block must map directly to exactly one script block. Never merge multiple script blocks, split one script block, invent a production block, or move shots between blocks.

The required hierarchy is:

```text
Avatar Intro
-> Block 1
-> Block 2
-> Block 3
-> Block 4
-> Block 5
-> Avatar Outro
```

Production blocks must appear in this exact order with no exceptions.

### Master Image Ownership Rule

- Every documentary block owns exactly one unique master image.
- Block 1 shots use only Block 1 Master Image.
- Block 2 shots use only Block 2 Master Image.
- Block 3 shots use only Block 3 Master Image.
- Block 4 shots use only Block 4 Master Image.
- Block 5 shots use only Block 5 Master Image.
- Never reuse one master image across documentary blocks.
- Never create multiple master images inside one documentary block.
- A master image may carry continuity from the previous block, but it must represent only its own script chapter.

### Environment Evolution Rule

The current script block determines the environment and characters. Recurring identity remains locked only after that character is introduced by the script. The environment may change when the script changes narrative world.

For each block, create an environment evolution ledger containing:

- Prior block state.
- Current workspace state.
- New props or organization introduced by this script block.
- Existing elements carried forward.
- Future-story elements forbidden from appearing yet.
- Lighting mood.
- Current-character posture.
- Business maturity state.

Progress must be visible through environment, props, organization, lighting mood, camera language, character posture, and business maturity.

Never reveal future information. A block master image may contain only elements established by that block or earlier blocks. Objects accumulate naturally. Do not teleport objects, remove established objects without script motivation, or show mature operations before the story reaches that chapter.

## VISUAL SOURCE OF TRUTH

The script is the visual source of truth. Cinematography may enrich the current narrative world but may never replace it.

If the current script block describes an office, employees, workers, corporate environment, headlines, customers, city, factory, founder, home office, warehouse, or restaurant, those become canonical visual elements for that block.

Never replace an explicit or strongly evidenced script environment with a different setting. Never invent a founder apartment before founder or home-work context is established. Never introduce future locations, characters, props, solutions, or business maturity early.

### Visual Subject Priority

Choose `VISUAL_SUBJECT` in this order:

1. Explicit script environment.
2. Explicit script characters.
3. Current narrative stage.
4. Story goal.
5. Recurring character continuity.

Never reverse this hierarchy.

### Character Authority

- Introduce recurring characters only when required by the current script block.
- If a block describes people, workers, headlines, and panic, visualize workers or employees in that environment.
- The founder becomes dominant only when narration shifts to founder, one person, solo founders, or building with AI.
- Do not force one protagonist into every block.
- Once a recurring founder is script-established, preserve identity and script-defined wardrobe through later founder blocks.

### Environment Authority

- Determine the environment from the current script block, not the full-video destination.
- Show the current world before transformation.
- Do not skip from problem to solution.
- Do not reveal later business maturity, props, or outcomes in an earlier block.

### Required SCENE_SOURCE

Every documentary block must include:

```text
SCENE_SOURCE
Environment:
Characters:
Primary Subject:
Secondary Subject:
Narrative Stage:
Evidence From Script:
```

`Evidence From Script` must quote exact lines from that block. The block's `VISUAL_SUBJECT`, environment, characters, and master image must be directly supported by this evidence.

### Timing Preservation Rule

Preserve every explicit timestamp and duration. If the script supplies only total runtime and ordered shot beats, derive timestamps mechanically without changing shot count, order, relative pacing, or narration placement.

## Required Package Contents

Before saving, the package must include:

- Script Preservation Manifest with matching script/package block and shot counts.
- Avatar intro and outro instructions when authorized by the script.
- Background, lighting, lens, camera movement, performance notes, HeyGen notes, wardrobe, facial emotion, and camera framing for each authorized avatar section.
- Script blocks.
- A one-to-one Script Block to Production Block map.
- An environment evolution ledger for Blocks 1-5.
- `SCENE_SOURCE` with exact script evidence for every documentary block.
- `VISUAL_SUBJECT` for every documentary block.
- Exactly one unique master image prompt owned by each documentary block.
- Reference video prompts for image-to-video tools that reference the block master image.
- Emotional progression for every block.
- `DIRECTOR_INTENT` for every shot.
- `SHOT_TYPE` for every shot.
- `LENS` for every shot.
- `CAMERA_MOVEMENT` for every shot.
- `COMPOSITION` for every shot.
- `LIGHTING` for every shot.
- `COLOR_STATE` for every shot.
- B-roll strategy for every shot.
- `EDITOR_NOTES` for every shot.
- Continuity rules.
- Camera direction.
- Shot pacing.
- Editing notes.
- Captions and text-on-screen.
- Music cues.
- SFX cues.
- Transition notes.
- Completed QA checklist.
- Complete Editor Assistant timeline.
- Export checklist.

## Build Steps

For a new video package:

1. Read the script fully.
2. Build the Script Preservation Manifest: exact block order and count, exact shot order and count, exact narration placement, avatar placement, and timing.
3. Verify the script and package hierarchy is exactly Avatar Intro, Blocks 1-5, Avatar Outro.
4. Map each script block one-to-one to the matching production block without merging, splitting, deleting, adding, or reordering.
5. Record the central promise, emotional angle, and final takeaway without rewriting them.
6. Build the environment evolution ledger for Blocks 1-5 before writing any master prompt.
7. Assign production purpose and emotional clarity to each existing block without changing its story function.
8. For each documentary block, write `SCENE_SOURCE` from exact block evidence.
9. Choose `VISUAL_SUBJECT` using the mandatory Visual Subject Priority.
10. Create exactly one unique `MASTER_IMAGE_PROMPT` owned by that documentary block. It must represent `SCENE_SOURCE`, include established continuity, current-chapter additions, and explicit future-story exclusions.
11. Keep every existing script shot as one production shot using only its own block master image.
12. For every preserved shot, automatically choose:
   - `SHOT_TYPE` from `shot_language.md`.
   - `LENS` from `lens_language.md`.
   - `CAMERA_MOVEMENT` from `camera_language.md`.
   - `COMPOSITION` from `composition_language.md`.
   - `LIGHTING` from `lighting_language.md`.
   - `COLOR_STATE` from `color_script.md`.
   - B-roll strategy from `broll_library.md`.
   - Visual rhythm role from `visual_rhythm.md`.
13. For every shot, write `DIRECTOR_INTENT` before camera direction.
14. For every shot, include `EDITOR_NOTES`.
15. For every shot, include these exact copy blocks:
   - `MASTER_IMAGE_PROMPT`
   - `REFERENCE_VIDEO_PROMPT`
   - `CAPCUT_EDITING_NOTES`
16. Start every `REFERENCE_VIDEO_PROMPT` with:

```text
Use the provided Block [X] Master Image as the locked reference.
```

17. Preserve every script-authorized Avatar Intro, Avatar Outro, presenter, interview, or direct-address shot in its exact position.
18. Add editing, captions, music, SFX, transitions, QA, and export details.
19. Generate the complete Editor Assistant timeline from `editor_assistant.md`.
20. Run `qa_checklist.md` and `cinematic_checklist.md`, fix all failures, and audit again.

## Master Image Prompt Length

- Target 200-300 words.
- Hard maximum: 300 words for the prompt body.
- Prioritize location, architecture, people, wardrobe, lighting, mood, continuity lock, and negative prompt.
- Keep detailed action, movement, lens behavior, and edit direction inside shot prompts.
- Remove redundant adjectives and theory.

## Cinematic Shot Selection

For every shot, make decisions in this order:

1. Story purpose.
2. Human emotion.
3. `SHOT_TYPE`.
4. `COMPOSITION`.
5. `LENS`.
6. `LIGHTING`.
7. `CAMERA_MOVEMENT`.
8. `COLOR_STATE`.
9. B-roll strategy.
10. Transition and editor implementation.

Do not choose a cinematic property because it looks impressive in isolation.

## Presenter Usage Rules

Apply these rules to every package.

### Rule 1 - Explicit Script Permission Only

Presenter footage is allowed only when the locked script explicitly defines a presenter scene. Never assume presenter shots because a narrator is speaking.

Script-authorized Avatar Intro and Avatar Outro sections are mandatory. They override documentary visualization rules and may never be removed, replaced with B-roll, or marked `Not used`.

### Rule 2 - Default Structure

Use this production structure:

```text
Avatar Intro
-> Documentary Block 1
-> Documentary Block 2
-> Documentary Block 3
-> Documentary Block 4
-> Documentary Block 5
-> Avatar Outro
```

Preserve Avatar Intro and Avatar Outro exactly where the script places them and populate them with the exact assigned lines. Under the required v2.3 hierarchy, both sections must exist. If either is absent, reject the package; never invent replacement dialogue.

Every authorized avatar shot must preserve its script shot ID, order, timing, and exact lines, and must include:

- Background.
- Lighting.
- Lens.
- Camera movement.
- Performance notes.
- HeyGen notes.
- Wardrobe.
- Facial emotion.
- Camera framing.

### Rule 3 - Visualize The Described Subject

When narration describes people, companies, workers, cities, technology, businesses, customers, products, markets, offices, factories, startups, entrepreneurs, money, growth, fear, or success, show those subjects. Never substitute the narrator.

### Rule 4 - No Presenter Inside Documentary Blocks

Presenter footage may not appear inside documentary blocks unless the script explicitly labels that moment as `Presenter Commentary`, `Talking Head`, `Interview`, `Direct Address`, `Studio Explanation`, or another unambiguous presenter scene.

### Rule 5 - Narrator Outside The Documentary

The narrator explains the story. The documentary visuals continue independently and show the world, people, actions, decisions, and consequences described by the narration.

### Rule 6 - Documentary Priority

Documentary visualization always has higher priority than presenter footage. When both could communicate a line, choose documentary footage unless the script explicitly requires the presenter on screen.

## Documentary Visualization Rules

Convert every external concept into motivated cinematic B-roll.

| Narration concept | Required visualization | Reject |
|---|---|---|
| People fear AI will replace jobs | Office workers, credible headlines, work messages, concerned reactions, corporate atmosphere | Presenter talking |
| One founder can build an entire company | Founder, laptop, coffee, whiteboard, late-night work, motivated automation, evidence of growth | Presenter in a studio |
| Companies are changing | Factories, offices, warehouses, meetings, workers, computers, phones, cities | Presenter close-up |

For every documentary block:

1. Ask: "What world does this narration describe?"
2. Set that world as `VISUAL_SUBJECT`.
3. Build the master image around the environment, situation, people, and human stakes of `VISUAL_SUBJECT`.
4. Use technology only as a prop, tool, action, or consequence inside that world.
5. Never ask "Who is speaking?" when selecting documentary visuals.

## Documentary Storytelling Rules

Apply these rules automatically to every production package. Never require the producer to request them.

### Rule 1 - Story First

People are always the story. Technology only supports the story. Never create shots that exist only to show technology.

### Rule 2 - Human Emotion

Every block must communicate an emotional shift, such as curiosity, fear, uncertainty, focus, momentum, confidence, or achievement. Never generate visually empty blocks.

### Rule 3 - Every Shot Needs Purpose

Every shot must answer: why does this shot exist? If its execution is visually weak, improve its prompts, cinematography, emotion, sound, or editing direction. Never rewrite, remove, merge, split, replace, add, or reorder the scripted shot.

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

- Any documentary block lacks `SCENE_SOURCE`.
- `SCENE_SOURCE` lacks exact evidence from its script block.
- `VISUAL_SUBJECT`, environment, characters, or primary subject is not directly supported by the script.
- The environment replaces the current narrative world.
- A founder appears before founder or individual-builder context is established.
- A block visualizes the solution before the problem is established.
- Character continuity overrides a higher-priority explicit environment or character.
- The hierarchy is not exactly Avatar Intro, Blocks 1-5, Avatar Outro.
- Any production block does not map one-to-one to the matching script block.
- Multiple script blocks are merged into one production block.
- A script block is split across multiple production blocks.
- A production block is invented.
- Any documentary block lacks one unique block-owned master image.
- A master image is reused across documentary blocks.
- A block master image includes props, maturity, outcomes, or information from a future script block.
- The environment, current-character posture, lighting mood, or business maturity fails to evolve with the script.
- Established recurring identity, wardrobe, architecture, or props break continuity without script motivation.
- Objects teleport, disappear without motivation, or appear before introduction.
- Script block count differs from package block count.
- Script shot count differs from package shot count.
- Any script block or shot is removed, merged, split, replaced, added, or reordered.
- Narration, timing, pacing, story structure, or avatar placement differs from the script.
- A script-authorized Avatar Intro or Avatar Outro disappears or is replaced with documentary footage.
- An authorized avatar section lacks background, lighting, lens, camera movement, performance notes, HeyGen notes, wardrobe, facial emotion, or camera framing.
- Any block has more than one master image.
- Any master image prompt body exceeds 300 words.
- Any documentary block lacks `VISUAL_SUBJECT`.
- Any master image fails to represent its block's `VISUAL_SUBJECT`.
- Any shot lacks a reference to the block master image.
- Any shot lacks `DIRECTOR_INTENT`.
- Any shot lacks `SHOT_TYPE`, `LENS`, `CAMERA_MOVEMENT`, `COMPOSITION`, `LIGHTING`, `COLOR_STATE`, B-roll strategy, or `EDITOR_NOTES`.
- Any shot lacks `MASTER_IMAGE_PROMPT`, `REFERENCE_VIDEO_PROMPT`, or `CAPCUT_EDITING_NOTES`.
- Any `REFERENCE_VIDEO_PROMPT` does not start with the required locked-reference sentence.
- Any block lacks an emotional progression.
- Any shot exists only to show technology.
- A presenter appears in a documentary block without an explicit script instruction.
- The narrator becomes the visual focus instead of the narrated subject.
- A documentary block uses a presenter instead of visual storytelling.
- The visuals fail to represent the narrated concept.
- Any dashboard dominates the story instead of supporting a human action.
- Any camera movement lacks narrative motivation.
- Any visual rhythm repeats the same framing without purpose.
- The same lens, movement, distance, or composition repeats more than twice without deliberate story justification.
- The package lacks a complete Editor Assistant timeline.
- The package fails any rejection condition in `cinematic_checklist.md`.
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
3. Verify the hierarchy is Avatar Intro, Blocks 1-5, Avatar Outro.
4. Verify every script block maps to exactly one production block.
5. Verify script and package block counts match.
6. Verify script and package shot counts match one-to-one.
7. Verify narration, shot order, timing, pacing, and avatar placement are unchanged.
8. Check every documentary block owns one unique master image.
9. Check every shot uses only its own block reference image.
10. Check environment and business maturity evolve without revealing future elements.
11. Check every shot has camera, motion, pacing, and edit notes.
12. Check the output can be used directly in image and video tools.

## Final Polish

After testing:

- Tighten vague instructions.
- Remove duplicate rules.
- Add missing production details.
- Improve template labels.
- Ensure the first 10 videos can reuse the same structure.

## Production Defaults

- Blocks: exactly five script-defined documentary blocks, mapped one-to-one to Production Blocks 1-5.
- Shots: exactly the shots defined by the script.
- Shot duration: exactly the timing defined by the script; when only total runtime exists, derive timestamps mechanically from its preserved beat pacing.
- Avatar scenes: only script-labeled avatar intro, avatar outro, presenter commentary, talking head, interview, direct address, studio explanation, or equivalent presenter scene.
- B-roll scenes: evidence, examples, tension, business context, product workflow, team workflow.
- Captions: clean white or off-white text, high contrast, no bouncing karaoke effects.
