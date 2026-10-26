# Robo DJ

A cute 3D robot that DJs behind a desk with two turntables during the breaks of your presentation. It dances, plays live-generated music and runs a light show while a countdown tells the audience when the talk continues.

The interface is in German. The tables below list every control with its English meaning.

## Getting started

Open `index.html` in a browser. There is no build step and nothing to install. three.js (0.149.0) and the fonts load from a CDN, so you need an internet connection.

To publish it with GitHub Pages: *Settings → Pages → Deploy from a branch → `main` / root*.

Browsers block autoplay with sound, so the music only starts after you click the play button.

## Features

### Music

All music is synthesized live in the browser with the Web Audio API. There are no audio files.

- **DJ-Set** (on by default): six original tracks built on the "four chords" of pop music, each with its own verse melody and chorus hook. The robot mixes them in a random order. Each track runs 32 bars: intro, verse, breakdown and build-up, chorus with a drop, and outro. Then the robot crashes into the next track, switching style and tempo.

  | Track | Style | Chords |
  |---|---|---|
  | Neon Kaffeepause | Pop, 116 BPM | I–V–vi–IV (C–G–Am–F) |
  | Slide 42 Anthem | House, 124 BPM | vi–IV–I–V (Am–F–C–G) |
  | Beamer Boogie | Funk, 104 BPM | I–V–vi–IV (G–D–Em–C) |
  | Retro Rakete | Retro disco, 112 BPM | I–vi–IV–V (D–Bm–G–A) |
  | Lo-Fi Folienwechsel | Lo-fi, 84 BPM | IV–I–V–vi (F–C–G–Am) |
  | Nächste Folie | Pop, 120 BPM | vi–IV–I–V (Em–C–G–D) |

- **Styles**: House, Retro-Disco, Lo-Fi, Funk and Pop. Clicking a style leaves the DJ set and plays endlessly generated music in that style. Every 16 bars a new section starts with its own chord progression, key, drum pattern, bass line, lead sound, melody and song form, plus drum fills, percussion layers, breakdowns and build-ups. Every press of play creates a new set.
- **Auto-Mix**: switches the style every 32 bars when playing generated music.
- **Sliders**: tempo, volume and a DJ filter (left: low-pass, center: off, right: high-pass).
- The top-left corner shows what is playing, e.g. "♪ Beamer Boogie · Refrain · I–V–vi–IV".

### Dance moves (Tanz)

| Button | Move |
|---|---|
| Auto | Changes the move every 4 bars |
| Auflegen | DJing: scratching and turning knobs |
| Hände hoch | Hands up |
| Robot Dance | Robot dance |
| Headbang | Headbanging |
| Pirouette | Spin |
| Winken | Waving |
| Disco-Finger | Disco finger pointing |

The robot blinks, follows the mouse with its eyes and changes its face (hearts, stars, grin). Click it for a "boop".

### Lights and effects (Licht & Effekte)

Lichtshow (moving spotlights), LED-Wand (LED wall following the spectrum, club stage only), Laser, Discokugel (disco ball), Nebel (fog) and Stroboskop (strobe). The strobe flashes at most about twice per second and is disabled when the system setting "reduce motion" is on.

### FX pad

Konfetti (confetti), Air-Horn, Scratch, and Drop (builds tension and hits on the next bar).

### Break timer (Pausen-Timer)

Set the banner text and a countdown of 5 to 30 minutes. The banner shows the time left and when the talk resumes. When the time is up, it reads "Weiter geht's!" ("Let's continue!"), the robot waves and the music fades out.

### Stage (Bühne)

- **Club**, **Strand** (beach at sunset with palm trees and string lights) or **Weltall** (space with a planet, a moon and a UFO).
- Custom text or your own logo (PNG, JPG, SVG) on the front of the DJ desk.
- The browser remembers stage, text, logo and other settings.

### Presentation mode

"Vollbild" switches to fullscreen. "Steuerung aus" hides the controls so only the stage and the banner remain.

## Keyboard shortcuts

| Key | Action |
|---|---|
| Space | Play / pause music |
| 1–8 | Choose dance move |
| J | DJ set on/off |
| . | Next track |
| M | Auto-Mix on/off |
| G | Change stage |
| S / W / L / D / N / B | Light show / LED wall / lasers / disco ball / fog / strobe |
| K / A / X / R | Confetti / air horn / scratch / drop |
| F | Fullscreen |
| H | Show / hide controls |
