# Free Retro 3D Effects

An explosion, a smoke column and a flame for low-poly 3D games, with six ready-to-use Godot 4 scenes. Each effect includes a soft, filtered N64-style scene and a hard-edged PS1-style scene. The pack also contains PNG flipbooks, frame data and SpriteFrames resources.

## Add to an existing Godot 4 project

1. Once this pack is approved in the Asset Library, open your project in Godot, find **Free Retro 3D Effects**, and install it into the project root. Until then, use the manual installation in step 2.
2. Keep the folder at `res://free-retro-3d-effects/`. The scenes and resources use that path. If downloading the repository manually, copy its `free-retro-3d-effects` folder into your project root; do not copy the outer repository folder into that location.
3. Let Godot import the textures. Drag an effect's `*-n64.tscn` or `*-ps1.tscn` scene into your 3D scene. For example, use `free-retro-3d-effects/explosion/explosion-n64.tscn`.
4. Run your scene. The effects use AnimatedSprite3D with billboard and autoplay enabled. The explosion plays once; the smoke and flame loop. Change **Pixel Size** to adjust their size.

This is an asset pack for an existing project, not a standalone demo project. Keep any existing copy of the folder safe before replacing it. The included `free-retro-3d-effects/README.txt` has the frame layout and additional engine instructions.

## More effects

The existing [Pixel Battle Effects Complete Collection](https://cs5475.itch.io/pixel-battle-effects-complete) contains the paid battle packs in the same style.

## License

See `LICENSE` and `free-retro-3d-effects/LICENSE.txt` for the license terms. The artwork is made with Puff; the tool itself is not included.
