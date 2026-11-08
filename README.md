# Sunset Dino Runner

A simple endless-runner game in a single HTML file: an orange dinosaur jumps green cacti across a sunset desert. The pace picks up as your score climbs.

## Play

Open `index.html` in any modern browser. No build step or install needed.

- **Space** or **↑**: jump (also starts and restarts the game)
- **↓**: drop faster while in the air
- **Tap** the game on a phone or tablet

Your high score is saved in your browser's local storage.

## Leaderboard

After a run, type a name and press **Save** to add your score to the shared top 10. Scores are stored in the Supabase table `dino_scores`, which anyone can read and add to but nobody can edit or delete through the game.
