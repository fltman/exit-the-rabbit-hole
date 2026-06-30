# Exit the Rabbit Hole

[![Support me on Patreon](https://img.shields.io/badge/Patreon-Support%20my%20work-FF424D?style=flat&logo=patreon&logoColor=white)](https://www.patreon.com/AndersBjarby)

A single-page WebGL animation that flies the camera through a twisting 3D tunnel and arrives at an image at the far end. The camera accelerates, holds at top speed, then decelerates to a stop facing the final slide — a small "exit the rabbit hole" presentation intro.

## What it does

- Builds a tube geometry along a custom sine/cosine curve with Three.js.
- Moves the camera and a point light along the path with an ease-in / hold / ease-out speed profile.
- Places `slideend.png` as a textured plane at the end of the tunnel as the reveal.

## Usage

Static page — open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

Note: the tunnel wall texture is loaded from `pattern.png`, which is not included in the repo; without it the tunnel renders plain white.

## Tech

Three.js (r128, loaded from CDN), WebGL, plain HTML.
