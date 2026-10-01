# SpaceBricks

A free, retro-flavored brick breaker with modern neon graphics and a head nod to classic arcade paddle games. Bounce the ball, break glowing bricks, catch power-up capsules, blow up explosive bricks and beat a boss every fifth level, through endless procedurally generated levels.

**Play it in your browser:** https://nbwillcox.github.io/SpaceBricks/

Everything is generated in code: sprites are vector-drawn on the fly, and all sound effects and music are synthesized with the Web Audio API. There are no image or audio files and no build step. A sibling of [SpaceGalaShooter](https://github.com/nbwillcox/SpaceGalaShooter), [SpaceCentiShooter](https://github.com/nbwillcox/SpaceCentiShooter), [SpaceVaderShooter](https://github.com/nbwillcox/SpaceVaderShooter), [SpaceStroids](https://github.com/nbwillcox/SpaceStroids), [SpaceCommand](https://github.com/nbwillcox/SpaceCommand), [lightCycles](https://github.com/nbwillcox/lightCycles) and [SpaceRoboShooter](https://github.com/nbwillcox/SpaceRoboShooter), with the same look and feel.

## Controls

| Action | Keys |
| --- | --- |
| Move the paddle | Mouse, or `A` / `D` / `←` / `→` |
| Launch the ball / release a caught ball / fire the laser | Left mouse button or `Space` |
| Pause | `P` or `Esc` |

## Gameplay

- Where the ball hits the paddle sets its bounce angle, and the ball speeds up as you break bricks and climb levels. Lose all balls and you lose a life (3 to start, extra lives at 20,000 and every 50,000 points).
- **Bricks:**
  - **Normal** bricks break in one hit.
  - **Armored** bricks take 2 or 3 hits and crack as they weaken.
  - **Gold** bricks are indestructible obstacles. (If a level stalls, the gold melts into armor so you can never get stuck.)
  - **Explosive** bricks blow up their neighbours in a chain reaction.
- **Capsules** drop from bricks:
  - **L** Laser
  - **C** Catch (sticky paddle)
  - **E** Enlarge
  - **S** Slow ball
  - **M** Multi-ball
  - **F** Fireball (smashes straight through bricks)
  - **N** Safety net (saves the next ball you drop)
  - **B** Bomb
  - **W** Warp (skips the level)
  - **1UP** Extra life
- **Drifters** are small drones that wander down the field. They knock the ball off course and explode when hit, so shoot or ram them for points.
- Chain brick hits without touching the paddle for a score multiplier (up to x8).
- **Bosses** appear every 5th level: shield, cannon or spawner guards must be broken before the core can be damaged. Their bolts cost you a life if they hit the paddle.
- Levels are endless: mirrored geometric layouts and pixel-art shapes alternate, with more armor, explosives and gold as you go. A new theme every 5 levels.
- Local top-10 high scores with arcade-style 3-letter initials (stored in your browser).

## Run locally

It is plain HTML/CSS/JS. Either open `index.html` directly, or serve the folder:

```bash
python -m http.server 8000
```

then visit http://localhost:8000. Desktop browsers with keyboard and mouse only for now. Add `?stage=N` to the URL to start at level N.

## License and attribution

Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): free to play, share and remix **non-commercially**, as long as you give credit and **link back to this repository**: https://github.com/nbwillcox/SpaceBricks

This is an original game inspired by classic arcade paddle games. It uses no assets, names or code from any existing game.
