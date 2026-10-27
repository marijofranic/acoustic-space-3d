# Acoustic Space 3D

A minimal browser-based audio visualization prototype. This repository preserves the uploaded `cartesian-sequencer.html` without code changes.

## Run

Open `cartesian-sequencer.html` in a browser. The page loads React 18, ReactDOM, Babel Standalone, Three.js r128, OrbitControls, and IBM Plex Mono from external services, so an internet connection is required. For microphone use, serve the page on localhost or HTTPS and grant microphone permission.

## Controls

- Mic: visualize microphone input.
- Audio: select a local audio file, which plays in a loop.
- Iso / Front / Side / Top: switch camera views.
- Auto: toggle automatic orbit.
- Fade: adjust retained trail length from 150 to 2000 points; this is not a time-based fade.
- Rec / Stop: capture the canvas and available audio as a WebM recording where supported.
- Clear: clear the visual trail.

## Mapping

- X: spectral spread, clamped at 2048 Hz.
- Y: estimated pitch, logarithmically mapped from 1000 to 9000 Hz.
- Z: scaled RMS amplitude, displayed as volume percentage.
- Colour: pitch.

## Status and limitations

This is an experimental prototype, not a calibrated acoustic measurement tool. This uploaded version does not include bird presets, a bird dropdown, shuffle/loop sequence controls, or the later proposed inward point projection. No browser testing was performed as part of this upload. GitHub Pages is not enabled by this commit.
