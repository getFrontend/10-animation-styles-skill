# Animation Styles Skill

An Agent Skill for creating short animated story videos with ten hand-built visual styles. It guides an agent through story planning, scene implementation, and local MP4 rendering.

## Included styles

| Style | Description |
| --- | --- |
| Pixel art | Low-resolution sprites, limited colors, and a game HUD |
| PS2 style | Low-poly 3D, small textures, fog, and a mission HUD |
| Comic art | Ink outlines, halftone dots, action lines, and caption boxes |
| Brick | A world built from toy-like bricks and studs |
| Claymation | Rounded clay shapes with stop-motion movement |
| Paper cutout | Layered paper shapes, shadows, and stepped animation |
| Retro anime | Cel-inspired color, speed lines, and impact frames |
| Low poly 3D | Faceted shapes and hard directional lighting |
| Risograph | Two-color halftone printing with imperfect registration |
| Miniature diorama | A small handmade set with tilt-shift depth of field |

See [`styles.md`](styles.md) for the visual rules and guidance for adapting each style.

## Install

Install the skill from GitHub with the standard Skills CLI:

```bash
npx skills add getFrontend/10-animation-styles-skill
```

The CLI installs the skill for the selected agent. TRAE users can install it through the same command and select TRAE when prompted.

## Use

Ask your agent to create an animated story video, then follow the workflow in [`SKILL.md`](SKILL.md). The skill helps plan the beats and styles, adapt the scenes, inspect rendered stills, and produce the final video.

The supporting references are:

- [`copywriter.md`](copywriter.md): story and beat-writing guidance
- [`styles.md`](styles.md): visual rules for the ten styles
- [`template/`](template/): runnable rendering project and example story

## Requirements

- Node.js and npm to install the template dependencies and run the renderer
- FFmpeg to encode MP4 video
- Python 3 and an ElevenLabs API key only when generating optional narration

The template can render still images without FFmpeg. It loads display fonts from Google Fonts, so internet access is needed for those fonts.
