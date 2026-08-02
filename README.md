# Piano Interval Ear Trainer

Train your ear to recognize musical intervals — from unison up through the
13th — played on a realistic sampled grand piano.

**Live app:** https://alainfidahoussen.github.io/piano-app-trainer/

## Features

- Real piano sound: Salamander Grand Piano samples, played back through
  [Tone.js](https://tonejs.github.io/) with a touch of reverb — no
  synthesized tones.
- All 22 interval qualities from unison to major 13th, individually
  selectable (with "Simple only", "Compound only", "Common 12", and "All"
  quick-select presets).
- Harmonic (both notes together), melodic (one after another), or mixed
  playback, with ascending / descending / random direction for melodic
  questions.
- Multiple-choice answers, a visual keyboard that highlights the notes
  played, and score/streak tracking saved locally in your browser
  (nothing is sent to a server).

## Running it locally

This is a single self-contained `index.html` file with no build step and
no dependencies to install. To try it locally:

```
python3 -m http.server 8000
```

then open http://localhost:8000/ in a browser. (Opening the file directly
via `file://` mostly works too, but some mobile browsers sandbox local
files and block JavaScript — a local server or the live GitHub Pages URL
above is more reliable, especially on iOS.)

## Deployment

Pushing to `main` triggers `.github/workflows/deploy.yml`, which publishes
the site to GitHub Pages (Actions deployment source).
