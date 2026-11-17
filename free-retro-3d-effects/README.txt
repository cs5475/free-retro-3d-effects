FREE RETRO 3D EFFECTS
An explosion, a smoke column and a flame, packed for low-poly 3D games

What's in here
  explosion/ 8 frames at 12 fps, plays once
  smoke/     12 frames at 12 fps, loops
  flame/     12 frames at 12 fps, loops

Each effect is a 4 x 4 flipbook: one 128 x 128 PNG holding 32 x 32 frames,
left to right, then top to bottom (empty cells at the end stay clear).
Small and power-of-two, the way a Nintendo 64 texture had to be.

Three copies of every flipbook:
  <name>-atlas.png        full color, soft alpha
  <name>-atlas-1bit.png   alpha is either on or off (hard edges, no sorting
                          trouble, the PS1 look)
  <name>-atlas-tint.png   grey, so you can tint it any color in a material
The JSON next to them has the frame size, count, grid, fps and loop.

The look
  N64: set the texture filter to Linear. The 32 px frames go soft, the way
  a filtered N64 texture did.
  PS1: set it to Nearest and use the 1-bit copy. Hard texels, hard edges.

Godot 4
  Each folder has two ready scenes: <name>-n64.tscn (Linear filter) and
  <name>-ps1.tscn (Nearest, 1-bit). Drop one in your 3D scene. They are
  AnimatedSprite3D nodes with billboard on, unshaded and autoplay, 32 px =
  1 unit (change Pixel Size to scale). The N64 scene blends the soft alpha;
  the PS1 scene cuts it hard. The .tres files are
  the SpriteFrames, if you'd rather build your own node.
  Keep the folder as it is, at res://free-retro-3d-effects/,
  or fix the paths.

Unity
  Import the atlas (Texture Type: Default, Alpha Is Transparency on,
  Filter Mode: Bilinear for N64 or Point for PS1, Compression: None).
  On a Particle System, turn on Texture Sheet Animation: Tiles X 4,
  Tiles Y 4, Frame over Time from 0 to frame_count / 16. Use an Unlit
  particle material (Additive suits the explosion and flame).

Other engines
  Any flipbook or sprite-sheet animation that takes a 4 x 4 grid.

License
  CC0 1.0. Use them for anything, no credit needed. See LICENSE.txt.

Where they come from
  These are frames from two free CC0 packs, repacked for 3D:
  Free Pixel Effects  https://cs5475.itch.io/free-pixel-effects
  Free Pixel Loops    https://cs5475.itch.io/free-pixel-loops
  Seven paid battle packs in the same style are in the Complete Collection:
  https://cs5475.itch.io/pixel-battle-effects-complete

How they were made
  Drawn by code with Puff, my pixel effect tool. No generative AI made the
  pictures.
