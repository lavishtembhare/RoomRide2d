# RoomRide2d

A Unity project (Unity 6000.0.58f2 / URP 2D) for **RoomRide2d** — appears to be a 2D-focused counterpart to the author's [`RoomRide`](https://github.com/lavishtembhare/RoomRide) project, set up from Unity's 2D URP scene template rather than the general/3D one.

## Current State

Like `RoomRide`, this repository is currently initialized from Unity's **"Unity Essentials"** learning-pathway template rather than containing custom RoomRide2d gameplay yet. `Assets/_Unity Essentials/` holds the stock tutorial scenes and scripts (kids' room, kitchen, living room, playground, top-down 2D, plus a 2D platformer `PlayerController2D`/`Collectible2D` pair). The project additionally includes `Assets/Settings/Scenes/URP2DSceneTemplate.unity`, confirming this was bootstrapped specifically from Unity's **2D (URP)** template rather than the standard 3D one used in `RoomRide`.

In short: this is another early-stage scaffold. It's a reasonable starting point for a 2D game, but the RoomRide2d-specific mechanics, art, and levels haven't been added on top of the template yet.

## Tech Stack

| Component            | Detail                                  |
|-----------------------|------------------------------------------|
| Engine               | Unity 6000.0.58f2                        |
| Render Pipeline      | Universal Render Pipeline (URP) 17.0.3, 2D template |
| Input                | Unity Input System                       |
| Camera               | Cinemachine 2.10.1                       |
| UI                   | UGUI + TextMesh Pro                      |
| Scripting            | C#                                        |

## Project Structure

```
Assets/
├── _Unity Essentials/         # Stock tutorial content (scenes, scripts, art, audio)
│   ├── Scenes/                 # Tutorial scenes (KidsRoom, Kitchen, LivingRoom, Playground, TopDown2D, etc.)
│   └── Scripts/                # PlayerController2D, Collectible2D, and other starter scripts
├── Scenes/
│   └── SampleScene.unity       # Default empty URP scene
├── Settings/
│   └── Scenes/URP2DSceneTemplate.unity  # The 2D URP template scene this project was seeded from
├── TextMesh Pro/                # TMP resources/fonts
└── InputSystem_Actions.inputactions
Packages/
└── manifest.json                # Package dependencies
ProjectSettings/                  # Unity project configuration
```

## Getting Started

1. Install **Unity Hub** and Unity Editor version **6000.0.58f2** (or a compatible newer 6000.x version).
2. Clone the repo:

   ```bash
   git clone https://github.com/lavishtembhare/RoomRide2d.git
   ```

3. In Unity Hub, **Add project from disk** and select the cloned folder.
4. Let Unity import assets and resolve packages (first import takes a few minutes).
5. Open `Assets/Scenes/SampleScene.unity` for the blank 2D starter scene, or explore the tutorial scenes under `Assets/_Unity Essentials/Scenes/`.

## Roadmap / Next Steps

- [ ] Add a dedicated `Assets/RoomRide2d/` folder for game-specific scripts, sprites, and scenes, separate from the tutorial content
- [ ] Build real 2D levels/scenes and register them in Build Settings
- [ ] Extend `PlayerController2D` with RoomRide2d-specific movement and interactions
- [ ] Add project-specific sprites, tilemaps, and UI
- [ ] Decide whether to keep the `_Unity Essentials` reference assets once no longer needed

## License

This project is licensed under **CC0 1.0 Universal** (public domain dedication) — see [LICENSE](LICENSE). Unity's own package/tutorial assets under `Assets/_Unity Essentials/` and `Assets/TextMesh Pro/` may carry their own licensing terms from Unity Technologies.
