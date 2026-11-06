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

## Local Development

```bash
npx http-server . -p 8080 -c-1
```
Then open http://localhost:8080