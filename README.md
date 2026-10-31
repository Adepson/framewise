# Framewise Storyboard Studio

A self-contained, offline-capable storyboard editor. Open `index.html` directly in a modern browser. No build step, external libraries, CDN fonts, or network connection are required.

## Features

- **Layered storyboard canvas:** Characters, props, effects, and backgrounds are separate selectable layers. Drag to move; use corner handles to resize and the top handle to rotate. Use the layer list to select elements and bring them forward or send them back.
- **Character library:** Standing, pointing, sitting, walking, running, jumping, and arms-crossed poses; happy, sad, angry, scared, surprised, and neutral expressions; short, long, curly, mohawk, and bald hairstyles; editable skin, hair, and clothing colors.
- **Props and effects:** Editable speech and thought bubbles, arrows, speed lines, dust clouds, and impact stars.
- **Backgrounds:** Day sky, night sky, interior room, street, graveyard, forest, and plain color presets. Each can be customized with a color picker.
- **Reusable assets:** Add assets from the library to any panel, then customize their pose, colors, text, size, position, rotation, and layer order.
- **Script-to-board:** Enter one action per line beginning with `PANEL:`. Each matching line adds a panel to the selected scene with the remaining text as its action note.
- **Scene management:** Add, rename, delete, and reorder scenes.
- **Panel management:** Add, duplicate, delete, and reorder panels. Each panel stores its action, dialogue/caption, duration, camera move, shot size, and camera angle.
- **Shot planning:** Extreme close-up, close-up, medium, wide, extreme wide, two-shot, and insert shot sizes; eye-level, high, low, over-the-shoulder, POV, Dutch, aerial, and top-down angles. The shot table lists all panels across scenes and supports in-place edits.
- **Exports:** PNG of the selected panel, PNG grid of the entire storyboard, print-ready project, CSV shot table, full-project JSON download and JSON load, and WebM animatic recording (where the browser supports `MediaRecorder` and canvas capture).
- **Animatics:** Play all scenes with per-panel timing, dialogue/action captions, static camera, slow zoom in, zoom out, pan left, or pan right.
- **Autosave:** Changes are saved to browser `localStorage` automatically. Use JSON save/load to keep portable backups or transfer projects between browsers.
- **Responsive dark interface:** Designed for desktop and smaller screens. All artwork is drawn with inline Canvas code; there are no external assets or dependencies.

## Keyboard shortcuts

- `N`: Add a panel to the current scene.
- `E`: Export the selected panel as PNG.
- `P`: Open and play the animatic.
- `Esc`: Close the animatic or shot-table overlay.

Shortcuts are ignored while typing in text fields and selectors.

## Data and privacy

Project data stays in the browser's local storage unless you explicitly export a JSON, PNG, CSV, printout, or WebM file. Clearing browser storage removes the local autosave, so keep a JSON backup for important work. Loading a JSON file replaces the project currently open in the editor.
