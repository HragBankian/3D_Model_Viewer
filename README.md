# 3D Model Viewer — UI/UX Design Challenge

An interactive web-based 3D model viewer prototype with all mandatory features + Dark/Light theme toggle.

## Live Demo

**[View the live app →](https://hragbankian.github.io/3D_Model_Viewer/)**

Hosted on GitHub Pages.

## Quick Start

```bash
# Option 1: Open index.html directly in a browser
# Option 2: Serve locally
npx serve -l 3000
# Visit http://localhost:3000
```

## Features

- **Model Upload & Info** — Drag-and-drop or click to upload `.glb`, `.gltf`, `.obj`; progress bar; vertex/triangle/mesh/material counts; dimensions
- **Performance Analysis** — Score (0–100), color-coded status, file size, texture memory, triangle count, optimization tips
- **Render Modes** — PBR, Wireframe, Normals, UV Checker, Unlit
- **Lighting Controls** — Main + Ambient light with intensity, color, reset
- **Camera Controls** — Front/Side/Top/3–4 presets; orbit/pan/zoom
- **3D Viewport** — Grid and axes toggles; responsive layout
- **Theme Toggle** — Dark/Light mode (optional feature)

See [DESIGN.md](DESIGN.md) for full design documentation.

## Deployment (GitHub Pages)

This project is deployed to GitHub Pages from the repository root:

1. Go to **Settings → Pages** in your GitHub repository
2. Under **Source**, select **Deploy from a branch**
3. Choose the `main` branch (or your default branch) and `/ (root)` folder
4. Save — the site will be available at `https://<username>.github.io/3D_Model_Viewer/`