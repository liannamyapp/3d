# Arka — 3D Chair Configurator

An interactive product configurator built with **Three.js (r128)** and plain JavaScript. No build step, no external models or images: the chair is assembled from primitives and all textures are generated at runtime.

**Live demo:** https://YOUR-USERNAME.github.io/arka-configurator/

![Demo](demo.gif)

## Features

- 6 upholstery options and 4 frame materials (oak, walnut, black metal, brass)
- Smooth color transitions between options
- Physically based materials (`MeshStandardMaterial`) with reflections from a PMREM environment built from emissive panels
- Procedural fabric and wood textures drawn on `<canvas>` (fabric texture doubles as a bump map)
- 3 lighting presets: studio, evening, daylight (ACES tone mapping, soft shadows)
- Toggleable armrests with animated transition
- Camera presets (front / 3/4 / side) animated along a sphere around the model
- OrbitControls with damping and optional auto-rotate
- Live SKU and dimensions update
- Responsive layout, light and dark themes, `prefers-reduced-motion` support

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Deploy to GitHub Pages

1. Push this folder to a new repository.
2. Go to **Settings → Pages**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The demo will be available at `https://<username>.github.io/<repo-name>/`.

## Tech

- [Three.js r128](https://threejs.org/) via CDN
- `OrbitControls` from `three/examples/js`
- Vanilla HTML, CSS and JavaScript in a single file

## License

MIT
