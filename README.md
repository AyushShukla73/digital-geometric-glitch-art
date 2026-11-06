# Digital Geometric Glitch Art Generator

A web-based image processing tool that transforms uploaded images through a geometric glitch pipeline.

## Live Demo

**https://ayushshukla73.github.io/digital-geometric-glitch-art/**

## Transformation Pipeline

1. **2×2 Mirror Grid** - Creates a 2×2 layout with:
   - Top-left: Original
   - Top-right: Horizontally mirrored
   - Bottom-left: Vertically mirrored
   - Bottom-right: Both mirrored

2. **Vertical Strip Recombination** - Splits into 40px vertical strips, then recombines by alternating from left and right edges inward

3. **Horizontal Strip Recombination** - Splits into 40px horizontal strips, then recombines by alternating from top and bottom edges inward

4. **Final Result** - Download the processed glitch art

## Usage

1. Click or drag & drop an image onto the upload area
2. Watch all intermediate steps render in real-time
3. Click "Download Final Image" to save the result

## Tech Stack

- Vanilla HTML/CSS/JavaScript
- HTML5 Canvas API for image manipulation
- No dependencies - runs entirely in browser

## Screenshots

| Step | Description |
|------|-------------|
| ![Step 1: 2×2 Mirror Grid](screenshots/step1-mirror-grid.png) | **2×2 Mirror Grid** — Original, horizontally mirrored, vertically mirrored, and both mirrored |
| ![Step 2: Vertical Strip Recombination](screenshots/step2-vertical-strips.png) | **Vertical Strip Recombination** — Split into 40px strips, recombined alternating from left/right edges |
| ![Step 3: Horizontal Strip Recombination](screenshots/step3-horizontal-strips.png) | **Horizontal Strip Recombination** — Split into 40px strips, recombined alternating from top/bottom edges |
| ![Step 4: Final Result](screenshots/step4-final-result.png) | **Final Glitch Art** — Downloadable result after all transformations |

*Add your screenshots to the `screenshots/` folder in the project root. The images above use relative paths that work on GitHub Pages.*

## Local Development

```bash
npx http-server . -p 8080 -c-1
```
Then open http://localhost:8080