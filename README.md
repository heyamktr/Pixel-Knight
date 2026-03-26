# Pixel Knight

Pixel Knight is a small 2D platformer built with Godot and GDScript. You control a pixel knight, collect coins, avoid hazards, use moving platforms, and reach the portal to continue to the next stage.

## Demo Video

Add your gameplay video here in either of these ways:

Hosted video link:

[Watch the demo](https://youtu.be/qURAf3fxYKg)

Local video file in the repo:

```md
https://github.com/your-username/your-repo/assets/your-video-id
```

If you want GitHub to show the video inline, upload the clip in the repository or issue comments first, then paste the generated GitHub asset URL above this section.

## Overview

- Built in Godot 4 with GDScript
- Main level starts in `scenes/game.tscn`
- Second level loads through a portal into `scenes/game3.tscn`
- Score system tracks coin collection out of 10
- Includes moving platforms, slime enemy patrols, hazards, sound effects, and background music
- Web export files are already present in `docs/`

## Gameplay

The player moves through a side-scrolling pixel-art map, collects coins, avoids falling into the killzone, and dodges a roaming slime enemy. Reaching the portal advances the player from the first level to the next scene.

## Controls

| Input | Action |
| --- | --- |
| `A` / `Left Arrow` | Move left |
| `D` / `Right Arrow` | Move right |
| `W` / `Space` / `Up Arrow` | Jump |

## Features

- Responsive left-right movement and jumping
- Animated knight character with idle, run, and jump states
- Coin pickup system with on-screen score tracking
- Moving platform section
- Enemy patrol behavior using raycasts
- Killzone reset when the player falls
- Level transition portal
- Web and Windows export presets

## Tech Stack

- Engine: Godot 4.6
- Language: GDScript
- Audio: MP3 and WAV assets
- Art: Pixel-art sprites, tilesets, and bitmap-style fonts

## Project Structure

```text
Pixel-Knight/
|-- assets/     # Sprites, fonts, music, and sound effects
|-- docs/       # Web export output
|-- scenes/     # Levels, entities, music scene, and reusable nodes
|-- scripts/    # Player, coin, enemy, killzone, and game manager logic
|-- project.godot
|-- export_presets.cfg
`-- README.md
```

## Run Locally

1. Open the project in Godot 4.
2. Load `project.godot`.
3. Press `F5` to run the game.

The configured main scene is `res://scenes/game.tscn`.

## Export

- Windows export preset outputs an executable build.
- Web export preset outputs to `docs/index.html`, which is useful for GitHub Pages hosting.

## Scripts

- `scripts/player.gd`: player movement, jumping, and animation switching
- `scripts/coin.gd`: coin pickup behavior and score updates
- `scripts/game_manager.gd`: score tracking and UI label updates
- `scripts/silme.gd`: enemy patrol movement
- `scripts/killzone.gd`: death/reset flow when the player falls
- `scenes/Portal.gd`: scene transition from level 1 to level 2

## Demo Section Template

Use this if you want a cleaner section later:

```md
## Demo Video

[Watch the demo](https://your-video-link-here)
```
