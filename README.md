# Domino Show

A domino study for Opus 5.5. 19,400 dominoes, every one of them real physics, set off by a single finger push.

**Watch it live: https://sam1983aing.github.io/domino-show/** (click to begin, sound on)

Made with Opus 5.5 in Claude Code.

## What it's made of

- **three.js** draws everything. The dominoes are drawn in batches, which is what lets a browser handle 19,400 of them.
- **Rapier**, a physics engine compiled to WebAssembly, gives every domino real weight and friction. Nothing is keyframed. The finger taps the first one and physics does the rest.
- **Plain JavaScript** lays out the course: lines, curves, forks, a spiral, stairs, a domino 20x taller than the rest, and big fields that hide a picture on the back of every domino, so the names appear as they fall.
- **A virtual camera operator** follows the exact domino that's falling and blends between shots so it plays as one long take.
- **Custom shaders** add depth of field, bloom and film grain.
- **Web Audio** makes every click live from the real collision forces. No sound files.

It's one HTML file with no build step. Open `index.html` in a browser (three.js and Rapier load from jsDelivr, so it needs a connection).

## Controls

Click to begin. **R** replay, **Space** pause, **M** sound, **T** timer, **D** the lab (orbit camera, tuning panel).

It's heavy: 19,400 physics bodies and a film-style render, so a recent laptop or desktop works best.

---

Imported from [Sam1983Aing/domino-show](https://github.com/Sam1983Aing/domino-show) — original code and attribution preserved.
