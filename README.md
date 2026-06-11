# Fable 5 Showcase

A small gallery of interactive demos written entirely by **Claude Fable 5** — Anthropic's frontier model — to show what it can build in pure HTML, CSS, and JavaScript. No frameworks, no libraries, no build step: every demo is a single self-contained file.

**Live site:** https://zhbchao.github.io/amazing_fable/

## The demos

| Capability | Demo | What's inside |
|---|---|---|
| 🎮 Game development | [Neon Breakout](games/) | Complete arcade game: combo scoring, armored bricks, particle explosions, screen shake, and a WebAudio synthesizer for sound effects |
| 🧊 3D graphics | [Software 3D Renderer](3d/) | A full 3D pipeline on a 2D canvas — six morphing tube meshes, iridescent/depth/solid shading, a bloom pass, parallax starfield, and per-face explosion physics that detonates and reassembles the surface |
| 🖋 SVG generation | [Infinite Landscapes](svg/) | Seeded procedural generator that assembles complete animated SVG documents — palettes, ridgelines, weather, wildlife — downloadable as standalone `.svg` files |
| 🎨 Generative art | [Flow Fields](generative/) | Thousands of particles painting through a hand-rolled fractal value-noise vector field, with curated palettes and PNG export |
| 🪢 Physics simulation | [Tearable Cloth](physics/) | Verlet integration with constraint relaxation: grab, fling, and rip the cloth; fibers glow red under stress and snap when overstretched |
| 📊 Data visualization | [Capability Graph](dataviz/) | Force-directed graph with spring forces, charge repulsion, drag interaction, and hover-to-trace highlighting |

## Running locally

It's all static — any web server works:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## How it was made

The entire site — concept, category selection, design system, and every line of code — was produced by Claude Fable 5 in a single session from one prompt:

> *build a github hosted website which will demonstrate the amazing capability of Claude Fable 5 model, including but not limited to games, 3D animation, SVG generation, etc.*

🤖 Generated with [Claude Code](https://claude.com/claude-code)
