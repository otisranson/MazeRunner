# MazeRunner

A small, dependency-free web maze generator, solver, and first-person walker.

Open `index.html` in a browser — no build step, no server, no npm.

- **Generator**: recursive-backtracker algorithm, four size presets
- **Solver**: BFS shortest path, shown as an overlay on the minimap via "Show Solution"
- **First-person view**: a Wolfenstein-style DDA raycaster rendered on `<canvas>`
  - Move: `W`/`S` or `↑`/`↓`
  - Turn: `A`/`D` or `←`/`→`
  - Strafe: `Q`/`E`
- Minimap inset shows the full maze, your position/heading, start (green) and exit (red)
- Reaching the exit shows a win banner with elapsed time
