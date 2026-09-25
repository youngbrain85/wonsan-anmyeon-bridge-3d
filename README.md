# Wonsan–Anmyeon Bridge 3D — Segment Review Viewer

A browser-based viewer (Three.js) for reviewing, segment by segment, the LOD4/5 3D model of the Wonsan–Anmyeon
Bridge (Solbit Bridge), a cable-stayed bridge with two diamond-shaped pylons.

- **Open the viewer**: https://youngbrain85.github.io/wonsan-anmyeon-bridge-3d/
- The interface is in Korean.

## What the model contains

Built and reviewed on July 13–15, 2026:

- The PY1 pylon in 32 parts (31 segments plus the refined pylon head), and the PY2 pylon as a single model mirrored
  from PY1 along the bridge axis
- 37 deck segments, colored as built (steel girders and cross beams, concrete slab)
- 72 stay cables with guide pipes and dampers; the cable anchorages were refined over several revisions against the
  drawings, quantity tables, installation drawings and close-up site photographs
- 8 bearings and 8 wind shoes
- Deck accessories — pavement, curbs, railings, barriers, drains and lighting poles — two rails for the under-deck
  inspection vehicle, and finger-type expansion joints at both ends
- 71 of the 73 models are marked as approved in the manifest (the exceptions are the PY1 pylon head, which was
  refined afterwards, and the mirrored PY2 model)

## Viewer features

- List of models with name, elevation range and review status (approved / under review); click a row to show or
  hide that model
- Wireframe display and translucent display of approved segments
- Section clipping along X and Y: drag a slider to see the interior of the hollow sections
- Model count and units shown on screen (meters; drawing dimensions in mm / 1000)

## Files

| Path | Contents |
|---|---|
| `index.html` | The viewer (Three.js modules in `lib/`) |
| `manifest.json` | List of models with names, elevation ranges and approval status |
| `models/*.glb` | 73 models: 37 deck segments, 32 PY1 parts, PY2, and one file each for the cables, bearings and deck furniture |
| `models/*_measure.json` | Measurements of the PY1 pylon segments: bounding box, watertightness, volume and cross-section slices (outer bounds and voids) |
