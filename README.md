# Hyper-Fractal: Ultra-High-Definition 3D/4D Raymarching Engine

A real-time, browser-based WebGL 2.0 fractal exploration engine featuring procedural 3D/4D raymarching, cinematic lighting, Web Audio reactivity, and 6-DOF drone navigation.

Built entirely as a zero-dependency, self-contained single-page application.

---

## Features

### 1. Fractal Topologies
- **Infinite Mandelbox**: Box folding, spherical folding, scale inversion, and architectural columns.
- **4D Quaternion Julia**: Dynamic $W$-slice morphing in 4-dimensional hypercomplex space ($q \to q^2 + C$).
- **Classic Mandelbulb**: High-order 8th-power spherical coordinate hypercomplex polynomial.
- **Apollonian Gasket**: Spherical Apollonian gasket sponge with infinitely nested Apollonian packings.

### 2. Cinematic Lighting & Shading
- **Analytical Soft Penumbra Shadows**: Evaluated along distance-field ray paths using improved smooth penumbra formulations.
- **Volumetric Crevice God-Rays**: Crevice dust haze and Mie-scattering light shafts inside cavernous structures.
- **ACES Filmic Tonemapping**: High dynamic range color compression with subtle edge chromatic aberration.
- **Multi-Channel Orbit Traps**: Geometric plane traps ($\min |z_{xyz}|$) mapping procedural circuit-board traces and biomechanical veins alongside sphere origin traps ($\min |z|^2$).
- **Procedural Studio HDRI**: Specular Blinn-Phong highlights, Fresnel rim-lighting, and ambient environment reflections.
- **Temporal Progressive MSAA**: Halton $(2, 3)$ subpixel camera jitter accumulation when idle for pristine anti-aliasing.

### 3. Web Audio Reactivity
- **Audio Inputs**:
  - **Live Microphone**: Capture environmental sound / music with real-time FFT frequency decomposition.
  - **Internal Drone Synth**: Generative 5-voice ambient synthesizer with resonant low-frequency oscillation.
- **Banded Frequency Modulation**:
  - **Sub / Bass**: Modulates 4D Julia $W$-slice and fractal folding parameters.
  - **Mid / High**: Drives emissive circuit veins, specular sparkle, and bloom intensity.
- **Integrated HUD Spectrum Analyzer**: Real-time frequency bar and waveform display.

### 4. Dual Camera System & Immersion
- **Orbit Mode**: Intuitive mouse/touch drag rotation and smooth pinch-to-zoom.
- **6-DOF Drone Flight Mode**: First-person interior flight through tunnels and caverns using an on-screen virtual joystick, altitude elevators, and mobile DeviceOrientation gyroscope steering.
- **Mobile Proximity Haptics**: CPU-side distance field collision detection triggering device vibration (`navigator.vibrate()`) when approaching fractal walls.
- **Cinematic Autopilot**: Pre-calculated smooth spline trajectory guiding the camera through internal hollows.
- **4K Super-Sample PNG Export**: One-tap offscreen rendering up to 3840×2160 resolution for ultra-high-definition wallpapers.

---

## Quick Start

No dependencies or build steps required. Simply serve the directory with any static HTTP server:

```bash
# Using Python 3
python3 -m http.server 8080

# Or using Node.js / npx
npx serve .
```

Open `http://localhost:8080` in any browser with WebGL 2.0 support (Chrome, Firefox, Safari, Edge).

---

## Controls

| Action | Orbit Mode | Drone Flight Mode |
|---|---|---|
| **Rotate / Look** | Left Mouse Drag / Touch Drag | Right Mouse Drag / Gyroscope Tilt |
| **Move / Fly** | Right Mouse Drag (Pan) | Virtual Joystick / `W`, `A`, `S`, `D` |
| **Altitude** | Mouse Wheel / Pinch Zoom | `Space` (Up) / `C` or `Shift` (Down) |
| **Toggle HUD** | Click `Hide / Show HUD` | Click `Hide / Show HUD` |
| **Autopilot** | Toggle `Cinematic Autopilot` | Toggle `Cinematic Autopilot` |
| **Capture Wallpaper** | Click `Export 4K Screenshot` | Click `Export 4K Screenshot` |

---

## License

MIT
