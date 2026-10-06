# Room from photos: site

A form in front of the `room-from-photos` engine. You upload photos, enter the room's size, doors, windows and furniture, and the page builds the 3D room, plan and fit checks from them.

The engine does not read photos by itself. In the skill, an agent turns photos into the `CONFIG` block; here you fill that block in through the form instead. Photos are shown in the engine's Photos panel, where you tune the camera until the model lines up.

## Run

From the repo root:

```bash
python3 -m http.server 8000
```

Open http://localhost:8000/site/. The page loads `skills/design/room-from-photos/starter.html` and its `textures/`, so serve the repo root, not `site/`. Three.js and the fonts load from CDNs, so it needs internet.
