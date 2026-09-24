# Summit Sales Countdown

A single-file, projector-friendly countdown for live sales goals. Set a target, count it down automatically or by hand, and celebrate with looping confetti, fireworks, and a brass fanfare when you hit zero.

No build step, no dependencies. Just open `summit-countdown.html` in a browser.

## Features

- **Big-screen display.** The number is sized for projectors, with a progress bar showing how much of the goal is done.
- **Auto or manual countdown.** Tick down on a timer, or step it by hand with −1 / +1.
- **Final stretch.** In the last 10, the number turns gold and pulses.
- **Celebration at zero.** Confetti, fireworks, and a synthesized fanfare loop until the page is closed or reset.
- **Keeps its place.** The count is saved in the browser, so a refresh won't lose your progress.
- **Works offline.** Everything is self-contained. It falls back to system fonts without internet.

## Usage

1. Open `summit-countdown.html` in Chrome, Edge, Firefox, or Safari.
2. Click **Settings** to set the headline, starting number, label, tick interval, and sound.
3. Click **Save and restart**, then **Start countdown** or step it down manually.

> **Tip:** Click anywhere on the page once before the big moment. Browsers block audio until someone interacts with the page.

### Keyboard shortcuts

| Key | Action |
| --- | --- |
| `Space` or `↓` | Minus one |
| `↑` | Plus one |
| `P` | Play / pause auto countdown |
| `F` | Toggle fullscreen |
| `H` | Hide / show controls. Hover the bottom edge to reveal them while hidden |

## Settings

| Setting | Description |
| --- | --- |
| Headline | Title shown at the top and on the celebration screen |
| Starting number | The goal to count down from |
| Label | Text under the number, e.g. "deals to go" |
| Count down every | Seconds between automatic ticks (minimum 0.2) |
| Play sounds | Tick sounds and the fanfare |

**Save** keeps the current count. **Save and restart** resets the count to the starting number.

## Hosting

To host it on GitHub Pages, rename the file to `index.html` or link to it directly, then enable Pages in the repo settings.

## Tech

This is a single HTML file with vanilla JavaScript. Confetti is drawn on a Canvas, audio is generated with the Web Audio API, and state is saved in `localStorage`. Fonts are Big Shoulders Display and Figtree from Google Fonts. If `prefers-reduced-motion` is set, the animations are toned down.
