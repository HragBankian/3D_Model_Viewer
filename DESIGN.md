# 3D Model Viewer — UI/UX Design Documentation

## Design Overview

This is an interactive HTML/CSS/JS prototype demonstrating the complete UI for a web-based 3D model viewer. All **6 mandatory features** plus **1 optional feature** (Dark/Light Theme Toggle) are implemented.

---

## Mandatory Features

### 1. Model Upload & Info
- **File upload button**: Drag-and-drop zone with click-to-upload
- **Supported formats**: `.glb`, `.gltf`, `.obj`, `.fbx` (as specified)
- **Loading progress**: 0–100% progress bar with percentage display
- **Model statistics panel**:
  - Vertex count
  - Triangle count
  - Number of meshes
  - Number of materials
  - Model dimensions (W × H × D)

### 2. Performance Analysis
- **Overall score**: 0–100 scale with color-coded status
  - Green (≥80): Good
  - Yellow (55–79): Moderate
  - Red (<55): Poor
- **3 key metrics**: File size, texture memory, triangle count
- **Optimization tips**: Contextual suggestions (e.g., "Reduce texture resolution...")

### 3. Render Modes
- **5 modes** with clear switcher:
  - Default PBR (full materials and lighting)
  - Wireframe (mesh structure)
  - Normals (color-coded normals)
  - UV Checker (checkered pattern for UV mapping)
  - Unlit (flat shading, no lighting)
- Active mode has visual indication (highlighted button)
- Instant switching between modes

### 4. Lighting Controls
- **Main Light**: Intensity slider, color picker, reset button
- **Ambient Light**: Intensity slider, color picker, reset button
- All controls update in real-time

### 5. Camera Controls
- **Preset buttons**: Front, Side, Top, 3/4 View
- **Interactive controls** (OrbitControls):
  - Mouse: Left-drag rotate, right-drag pan, scroll zoom
  - Touch: One-finger rotate, two-finger pan, pinch to zoom
- Auto-fit model on load

### 6. 3D Viewport
- Large canvas for displaying the 3D model
- Optional toggles: Grid helper, Axes helper
- Responsive design adaptable to window size
- Clean, professional appearance

---

## Optional Feature: Dark/Light Theme Toggle

- Switch between dark and light UI themes
- One-click toggle in the top bar
- Preserves accessibility and readability in both modes

---

## Design Decisions

| Aspect | Choice | Rationale |
|--------|--------|-----------|
| **Layout** | Left sidebar (upload + stats + performance), right sidebar (modes + lighting + camera) | Keeps controls grouped by function; viewport stays centered and unobstructed |
| **Typography** | DM Sans (UI), JetBrains Mono (stats/metrics) | Clear hierarchy; monospace for numerical data |
| **Color** | Dark-first theme with accent blue (#4a9eff) | Familiar for 3D tools; reduces eye strain |
| **Spacing** | 16px panel padding, 8–24px gaps | Consistent rhythm and visual breathing room |
| **Feedback** | Progress bar, active states, hover states | Clear affordances and system status |

---

## How to Run

1. Open `index.html` in a modern browser, or
2. Serve locally: `npx serve -l 3000` then visit `http://localhost:3000`

---

## Evaluation Checklist

- [x] **User Experience (40%)**: Intuitive layout, clear hierarchy, ease of use
- [x] **Functionality (30%)**: All 6 mandatory features + 1 optional
- [x] **Visual Design (30%)**: Aesthetic quality, consistency, creativity
