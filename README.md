# Gravity Maze / 重力迷宫

Play: https://myechos.github.io/gravity-maze-demo/

A single HTML file, with no backend or external dependencies.

- Mobile: grant device orientation permission and calibrate. HTTPS is required.
- PC: choose rotation mode and drag the board horizontally. The ball falls toward the bottom of the screen.
- Collect numbered checkpoints in order before entering the center hole.
- Hitting a red spiked wall fails the attempt. Stepped border notches are ordinary solid obstacles.
- Failure, manual retry and mode switching retain the current layout and restart checkpoint collection.
- Success advances to a new random level; reloading starts at level 1.

Difficulty alternates, changing one dimension at a time:

1. Level 2: increase total wall length by 22.5 (5% of initial total).
2. Level 3: add a checkpoint.
3. Level 4: turn an ordinary wall into an L shape, counted as two segments, preserving total length.
4. Level 5: replace an existing wall segment with a spiked segment.
5. Repeat this four-step cycle.

Caps: 1100 total wall length, 12 checkpoints, 10 segments (5 L-shaped walls), and at most all segments spiked. Each segment is also limited to 115 to preserve navigable space. Capped upgrades leave the corresponding parameter unchanged. Layout connectivity includes wall shapes, spike clearance and irregular border notches. All checkpoints are generated in the reachable space.

Sensitivity and friction preferences are saved locally. Level progress is not saved.
