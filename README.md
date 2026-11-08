# Sunset Dino Runner

A simple endless-runner game in a single HTML file: an orange dinosaur jumps green cacti across a sunset desert, through four levels of rising difficulty.

## Play

Open `index.html` in any modern browser. No build step or install needed.

- **Space** or **↑**: jump (also starts and restarts the game)
- **↓**: duck on the ground, or drop faster in the air
- **Phone or tablet**: tap to jump, hold the bottom of the game to duck

## Coins and tokens

- **Gold coins**: worth half an obstacle's points at your current level (5, 10, 20 or 40)
- **Green gem** (rare): worth five obstacles' points
- **Shield** (rare): absorbs one crash

## Levels

You score points for each obstacle you clear. Each level brings new obstacles, more speed and more points per obstacle.

| Level | Name | Starts at | New obstacles | Points per obstacle |
|---|---|---|---|---|
| 1 | Desert Walk | 0 | Single cacti | 10 |
| 2 | Cactus Patch | 200 | Cactus clusters, rocks | 20 |
| 3 | Bird Alley | 600 | Low-flying birds (jump, duck or run under) | 40 |
| 4 | Dust Storm | 1,600 | Bouncing tumbleweeds, tighter gaps | 80 |

Your high score is saved in your browser's local storage.

## Leaderboard

After a run, type a name and press **Save** to add your score to the shared top 10, ranked from highest to lowest score, along with the level you reached. Scores are stored in the Supabase table `dino_scores`, which anyone can read and add to but nobody can edit or delete through the game.
