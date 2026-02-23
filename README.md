# RetroGames

A collection of classic retro arcade games recreated in modern TypeScript with Canvas 2D / WebGL. Each game is a faithful rendition of the original's spirit, gameplay, and AI — built with zero runtime dependencies, procedural audio via Web Audio API, and pixel-perfect rendering scaled for modern displays.

## Games

| Game | Year | Developer | Repo | Status | Description |
|------|------|-----------|------|--------|-------------|
| [Pac-Man](https://github.com/mmackelprang/PacMan) | 1980 | Namco | [PacMan](https://github.com/mmackelprang/PacMan) | Complete | The original maze chase game |
| [Tempest](https://github.com/mmackelprang/Tempest) | 1981 | Atari | [Tempest](https://github.com/mmackelprang/Tempest) | Complete | Vector tube shooter with 16 tube shapes |
| [Asteroids](https://github.com/mmackelprang/Asteroids) | 1979 | Atari | [Asteroids](https://github.com/mmackelprang/Asteroids) | Complete | Vector space shooter with Newtonian physics |
| [Battlezone](https://github.com/mmackelprang/Battlezone) | 1980 | Atari | [Battlezone](https://github.com/mmackelprang/Battlezone) | Complete | First-person wireframe tank combat |
| [Defender](https://github.com/mmackelprang/Defender) | 1981 | Williams | [Defender](https://github.com/mmackelprang/Defender) | Complete | Side-scrolling space shooter with humanoid rescue |
| [Night Driver](https://github.com/mmackelprang/NightDriver) | 1976 | Atari | [NightDriver](https://github.com/mmackelprang/NightDriver) | Scaffolded | First-person night racing |

## Common Tech Stack

All games share a common architecture derived from the PacMan reference implementation:

- **TypeScript** (strict mode) + **Vite** build system
- **HTML5 Canvas 2D** with software 3D projection for Battlezone
- **Web Audio API** procedural sound synthesis — no audio files
- **Zero runtime dependencies** — all graphics and sound generated procedurally
- **Fixed-timestep game loop** (60 FPS physics, variable render rate)
- **FSM-based game states** (Menu → Playing → GameOver)
- **Keyboard + touch input** with direction buffering

## Running Any Game

```bash
git clone https://github.com/mmackelprang/<GameName>.git
cd <GameName>
npm install
npm run dev
```

Open http://localhost:5173 in your browser.

## Discovery

All repos are tagged with [`retrogame`](https://github.com/mmackelprang?tab=repositories&q=retrogame) for easy discovery.

## License

ISC
