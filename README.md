# Fable 5 Showcase

A gallery of interactive pieces written entirely by **Claude Fable 5** — Anthropic's frontier model. Most demos are single self-contained HTML files; the centerpiece, *Genesis*, uses [three.js](https://threejs.org) loaded from a CDN. Everything runs as static files on GitHub Pages — no build step.

**Live site:** https://zhbchao.github.io/amazing_fable/

## The works

| # | Work | Capability | What's inside |
|---|---|---|---|
| 01 | [Genesis](3d/) | Three.js · GPU particles | 220,000 particles in one custom shader morphing between a spiral galaxy, Saturn, a torus knot, DNA, a Lorenz attractor, and type — simplex-noise turbulence, UnrealBloom post-processing, world-space cursor repulsion, orbit camera |
| 02 | [Little Path Tracer](raytracer/) | Ray tracing | A progressive path tracer in pure JS: global illumination, soft sun shadows, mirror and glossy materials, emissive night lamps — one jittered sample per pixel per frame, converging live |
| 03 | [Watch It Learn](neural/) | Machine learning | A multilayer perceptron with Fourier-feature inputs — forward pass, backpropagation, and Adam hand-written — trains live in the tab to paint a target image, including one you doodle yourself |
| 04 | [Endless Symphony](music/) | Generative music | An infinite composition: chords, bass, melody, and drums improvised from a seed, every instrument synthesized from raw oscillators through a hand-built reverb and delay |
| 05 | [Neon Breakout](games/) | Game development | Complete arcade game: combo scoring, armored bricks, particle explosions, screen shake, and a WebAudio synthesizer for sound effects |
| 06 | [Tearable Cloth](physics/) | Physics simulation | Verlet integration with constraint relaxation: grab, fling, and rip the cloth; fibers glow red under stress and snap when overstretched |
| 07 | [Flow Fields](generative/) | Generative art | Thousands of particles painting through a hand-rolled fractal value-noise vector field, with curated palettes and PNG export |
| 08 | [Infinite Landscapes](svg/) | SVG generation | Seeded procedural generator that assembles complete animated SVG documents — palettes, ridgelines, weather, wildlife — downloadable as standalone `.svg` files |
| 09 | [Capability Graph](dataviz/) | Data visualization | Force-directed graph with spring forces, charge repulsion, drag interaction, and hover-to-trace highlighting |

## Design

The site is set in [Fraunces](https://fonts.google.com/specimen/Fraunces), [Inter](https://fonts.google.com/specimen/Inter), and [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) — warm ivory on near-black with a single amber accent, film grain, and cursor-following previews on the index.

## Running locally

It's all static — any web server works:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

(Genesis fetches three.js from jsDelivr, so it needs a network connection.)

## How it was made

The entire site — concept, design system, shaders, and every line of code — was produced by Claude Fable 5 across two sessions. The second brief, in full:

> *the only goal is to demonstrate your strong capability. and please also design the pages with great taste. I don't like the current 3D demo, you may use three.js or any other library if it can be used. just WOW me.*

🤖 Generated with [Claude Code](https://claude.com/claude-code)
