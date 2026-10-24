# Space Calculus

A 2D Unity game that teaches functions by turning them into flight paths. You type a math expression on an in-game calculator, the game graphs it, and your spaceship flies along the curve. Reach the goal without getting pulled into a black hole.

## How it plays

1. Enter a function, such as `x^2 + 3x + 2`, on the calculator. Input is rendered as proper math notation as you type.
2. The function is plotted from the ship's position, and the ship follows the curve.
3. Black holes pull the path toward them and white holes push it away, so you have to account for them when choosing a function.
4. Touching a black hole sends the ship back to its last saved spot. Reach the goal to finish the level.

The grapher can also plot a function's first or second derivative.

## Scenes

| Scene | Purpose |
| --- | --- |
| `MainMenu` | Title screen |
| `Tutorial` | Tutorial level |
| `Calculator` | The main level with the calculator, grapher and hazards |

## Getting started

1. Install **Unity 6 (6000.1.4f1)** through Unity Hub.
2. Clone the repository and open the folder in Unity Hub.
3. Open `Assets/Scenes/MainMenu.unity` and press Play.

The project uses the Universal Render Pipeline with the 2D renderer and the Input System package.

## Project structure

| Path | Contents |
| --- | --- |
| `Assets/1Mine/Scripts/` | Game logic: grapher, spaceship, holes, goal, spawner |
| `Assets/1Mine/Scripts/LaTeXHandlers/` | Converts the calculator's math notation into a plottable function |
| `Assets/Scripts/UI/Calculator/` | Calculator input handling |
| `Assets/1Mine/Spriites/` | Game sprites |
| `Assets/Scenes/` | Game scenes |

## Built with

- [Unity 6](https://unity.com/) with URP 2D
- TEXDraw (Unity Asset Store) for rendering math notation
- [mXparser](https://mathparser.org/) for evaluating expressions
