# Interstellar Warp Sequence

Audio-reactive interstellar warp tunnel shader — runs entirely in-browser via WebGL/GLSL. No dependencies, no install.

## Features

- **3-layer interstellar tunnel** — depth-marched star fields blended and rotated independently per layer
- **Plasma warp texture** — electric filament pattern (ported from [4dG3zd](https://www.shadertoy.com/view/4dG3zd)) recolored as magenta/cyan plasma and depth-marched along the tunnel path
- **Nebula clouds** — fbm cloud field (ported from [4t2cR1](https://www.shadertoy.com/view/4t2cR1)) used as background nebula you fly through; only visible in darker regions of the tunnel
- **Energy streak flares** — nimitz-style flare fbm (ported from [4d2XR1](https://www.shadertoy.com/view/4d2XR1)) pulsing with bass hits
- **Full audio reactivity** — bass/mid/treble drive FOV breathing, bloom threshold, spin speed, camera shake, and streak intensity
- **Motion blur** — velocity-scaled blur along the tunnel direction
- **Feedback trails** — ping-pong framebuffer for trail/tracer effect
- **Inertial camera spin** — rotation starts at t=25s with drag physics, slowly accelerating
- **Performance** — renders at 0.72× resolution internally and blits cheaply to full screen

## How to Run

Just open `interstellar_warp.html` in any modern browser (Chrome/Firefox/Edge). No server needed.

1. Select a track from the dropdown
2. Press **Play**
3. Press **Restart** to reset the animation timeline back to t=0

## Credits

Portions of GLSL logic adapted from the following Shadertoy shaders:
- [Electric Flare (4dG3zd)](https://www.shadertoy.com/view/4dG3zd)
- [Sailing Beyond / Hyper Tunnel (4t2cR1)](https://www.shadertoy.com/view/4t2cR1)
- [Phoenix Flare (4d2XR1)](https://www.shadertoy.com/view/4d2XR1)
