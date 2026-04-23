# Generative Pattern Sketchpad

A low-code tool for creating animated generative art patterns — no coding required.
Adjust the controls, watch your pattern update live in the canvas, then export a
standalone HTML file you can share or host anywhere.

**[Open the tool → GenPatternSketchpadClaude.html](GenPatternSketchpadClaude.html)**

---

## How to Use

Open `GenPatternSketchpadClaude.html` in any modern web browser. No installation or
dependencies needed.

### Controls

| Control | What it does |
|---|---|
| **Pattern Mode** | Switch between Geometric (grid of shapes) and Particles (shapes drifting freely) |
| **Shape** | Choose Circle, Square, or Triangle |
| **Color Palette** | Warm, Cool, Monochrome, Rainbow, or Neon |
| **Density** | Number of shapes on screen |
| **Speed** | How fast shapes move and animate |
| **Size** | Scale of each shape |
| **Background** | Dark or Light canvas background |

### Buttons

- **Randomize** — Scrambles all settings at once. Good for discovering unexpected combinations.
- **Export HTML** — Downloads a self-contained `pattern.html` file with your current
  settings baked in. Open it in a browser, or upload it to GitHub Pages to share with others.

---

## About the Exported File

The exported `pattern.html` runs at full browser window size and is fully
self-contained — it loads p5.js from a CDN and needs no other files. You can:

- Open it directly in a browser
- Host it on GitHub Pages
- Upload it to any static file host

---

## Built With

- [p5.js](https://p5js.org/) — JavaScript library for creative coding
- Vanilla HTML, CSS, and JavaScript — no build tools or dependencies

---

## Course Context

Created for UCF ENG6819 as an extra credit project exploring low-code and no-code
creative tools. The tool demonstrates how a configured interface can generate working
p5.js code on behalf of the user — the user never writes code directly.
