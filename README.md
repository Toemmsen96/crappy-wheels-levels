# crappy-wheels-levels
Levels and replays for [Crappy-Wheels](https://toemmsen.ch/crappy-wheels).

The game's level browser lists every `.json` file directly inside `Base/` and `Community/`, so a level shows up in the game as soon as it is on `main`.

| Folder | |
| --- | --- |
| `Base/` | Levels that come with the game |
| `Community/` | Levels shared by players |
| `Replays/` | Replays of leaderboard times, in a folder per level |

## Submitting levels

Share a level from the game's level selector, which adds it to `Community/`, or make a pull request.

## Replays

When players finish a level with a leaderboard, they can upload the replay of their best time from the finish screen. Nothing is uploaded unless they choose to. The game's [backend](https://github.com/Toemmsen96/crappy-wheels-backend) commits it as `Replays/<level id>/<random id>.json`, and the leaderboard gets a Watch button next to that time.

Each player has at most one replay per level here: uploading a new one removes the old one in the same commit. A replay records the car's position, rotation and wheel rotations, and the controls held, 20 times a second through the run.

## License

The levels and replays in this repository are published under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/) (CC BY-NC-SA 4.0), see [LICENSE](LICENSE). Credit goes to the author named in each level file and the player named in each replay. By submitting a level, through a pull request or the Share button in the game, or by uploading a replay from the game, you agree to publish it under this license.
