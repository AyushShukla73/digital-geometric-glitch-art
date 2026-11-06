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

### Pipeline Steps

| Step | Preview | Description |
|------|---------|-------------|
| **Original** | ![Initial Image](screenshots/initial%20image.png) | Source image before processing |
| **Step 1: 2×2 Mirror Grid** | ![Complete 2×2 Grid](screenshots/Complete%202%C3%972%20Grid.png) | Original, horizontally mirrored, vertically mirrored, and both mirrored combined |
| **Step 2: Vertical Strips** | ![Split Vertical](screenshots/Split%20into%2040px%20vertical%20strips.png) | Split into 40px vertical strips |
| | ![Recombined Vertical](screenshots/Recombined%20(left,%20right,%20left%2B1,%20right-1...).png) | Recombined alternating from left/right edges |
| | ![Joined Vertical](screenshots/Joined%20result.png) | Joined vertical recombination result |
| **Step 3: Horizontal Strips** | ![Split Horizontal](screenshots/Split%20into%20horizontal%20strips.png) | Split into 40px horizontal strips |
| | ![Joined Horizontal](screenshots/Joined%20result.png) | Joined horizontal recombination result |
| **Step 4: Final Result** | ![Final Processed](screenshots/final%20processed%20image.png) | Final glitch art after all transformations |

*Images use URL-encoded paths that work on GitHub Pages. Add/replace screenshots in the `screenshots/` folder as needed.*

## Local Development

```bash
npx http-server . -p 8080 -c-1
```
Then open http://localhost:8080