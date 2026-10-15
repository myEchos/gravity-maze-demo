# Gravity Maze / 重力迷宫

Pure HTML5 maze: https://myechos.github.io/gravity-maze-demo/

- Mobile: enable orientation permission and calibrate; PC: drag to rotate the maze.
- Collect numbered checkpoints in order before entering the center hole.
- Failure, manual retry, and mode switching preserve the current level layout.
- Success advances to a new random level. Reload starts from level 1.
- Start with 4 checkpoints and 5 walls; every 4 completed levels adds one of each.
- Wall total length starts at 450 and increases by 22.5 per level (5% of the initial length).
- Fixed-board density limits: 12 checkpoints, 10 walls, total wall length 1100.
- Walls remain separated and layouts are checked for connectivity.
- Sensitivity and friction preferences are saved locally; level progress is not.

A single index.html with no backend or external dependencies. HTTPS is required for mobile sensors.
