# MazeRunner

A small, dependency-free web maze generator, solver, and first-person walker.

**[▶ Try it live](https://otisranson.github.io/MazeRunner/)** -- runs entirely client-side
(plain HTML/JS/canvas, no backend), so the GitHub Pages deploy is the real thing, not a demo.

Or open `index.html` in a browser directly — no build step, no server, no npm.

<img src="screenshots/screenshot.png" alt="MazeRunner: first-person raycast view of a hexagon-shaped maze, with the minimap and solution path shown in the corner" width="640">

- **Generator**: recursive-backtracker algorithm, four size presets
- **Shape**: Square, Circle, Triangle, or a regular Pentagon through Decagon — the maze is carved
  to fit any of them, with entrance/exit placed at opposite corners of the shape
- **Solver**: BFS shortest path, shown as an overlay on the minimap via "Show Solution"
- **First-person view**: a Wolfenstein-style DDA raycaster rendered on `<canvas>`
  - Move: `W`/`S` or `↑`/`↓`
  - Turn: `A`/`D` or `←`/`→`
  - Strafe: `Q`/`E`
- Minimap inset shows the full maze, your position/heading, start (green) and exit (red)
- Reaching the exit shows a win banner with elapsed time
