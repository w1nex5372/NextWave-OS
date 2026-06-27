# Editor Assistant

Purpose: convert the production package into a complete executable editing timeline.

Every final production package must include an Editor Assistant section after the Editing Plan.

## Required Timeline

Create a time-coded table with one row per shot:

| Time | Block | Shot ID | Master Reference | Video Track | Dialogue | Music | SFX | Subtitle | Transition | Speed | Color | Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|

Every documentary row must name its script block and that block's unique master image. Never assign a shot to another block's master image.

## Track Layout

### Video Tracks

- `V1`: primary documentary footage or explicitly scripted avatar footage.
- `V2`: B-roll, inserts, reaction shots, cutaways.
- `V3`: captions, text-on-screen, lower thirds.
- `V4`: adjustment layers, grain, masks, reframes when required.

### Audio Tracks

- `A1`: narration or avatar dialogue.
- `A2`: room tone and location ambience.
- `A3`: music master or stems.
- `A4`: spot SFX.
- `A5`: transition SFX and impacts.

## Required Editing Decisions

### Music Timing

- Cue start time.
- Stem or energy change.
- Music drop.
- Final fade.

### SFX Timing

- Exact frame or word cue.
- Perspective and level.
- Whether the effect bridges the cut.

### Subtitle Timing

- Exact in/out time.
- Maximum two lines.
- Highlight word or number.
- Safe-zone check.

### Speed Ramps

Specify start speed, ramp point, end speed, and story reason. Do not use by default.

### Zooms

Specify scale percentage and duration. Use only for reframing or emphasis that cannot be achieved through the source shot.

### Transitions

Specify transition type, duration, and motivation.

### J-Cuts And L-Cuts

Specify audio lead or tail duration. Use to connect scenes and preserve documentary flow.

### Hold Frames

Specify frame, duration, and reason. Use for final emphasis, evidence, or CTA only.

### Color Grade Notes

- Color state per block.
- Gradual cross-block lighting evolution.
- Exposure and skin-tone priorities.
- Contrast and saturation changes.
- Match notes between generated shots.
- Recurring character identity and wardrobe continuity after introduction; architecture and accumulated prop continuity only within recurring environments.

### Export Settings

- 9:16 vertical.
- 1080x1920 minimum or 2160x3840 preferred.
- H.264 or H.265.
- 24fps or 30fps.
- Audio peaks below -1 dB.
- Dialogue above music.

## CapCut Implementation Notes

- Build the timeline in story order on `V1`.
- Add B-roll to `V2` for motivated inserts, cutaways, and reactions. Do not reserve timeline space for avatar reactions unless the locked script explicitly requires presenter footage.
- Add captions on `V3` using one reusable style preset.
- Use keyframes only for specified reframes or moves.
- Use adjustment layers for consistent grade rather than grading every clip independently.
- Keep transitions short and restrained.
- Review once with sound off for visual clarity and once with picture hidden for audio flow.
