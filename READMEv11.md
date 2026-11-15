# Flight School – "How Flying Works: The 4 Forces of Flight"

Open any file directly in a browser (double-click). No server or build step is needed.

| File | What it is |
|---|---|
| `index.html` | Hub with links to the three pieces. If you publish the game itself as `index.html` on a website, its Home link hides itself. |
| `flying-poster.html` | One-page poster |
| `flying-website.html` | One-page website with a quiz |
| `flying-game.html` | The playable physics game (this README is mostly about it) |

## The game

Take off, climb, land softly and stop. Five levels, each teaching one idea
(calm air → headwind → gusts → heavy cargo → short runway).

### What's new in v11
- **The runway is placed when you reach the target height.** It sits `LEVEL_U` (1,100 units, about 5,000 ft) of level flight ahead plus the distance the 3.5° path needs to come down from the target height (`placeRunway()`). It fits any climb rate, so the lights come on at "on path" and not "too high". Before you reach the target there is no landing runway.
- **Missed approach:** if you fly past the end of the runway in the air, the flight ends with a "Missed approach" result and a tip using your height at the aim point. Nobody crashes.
- **Grass after take-off:** touching the grass again after lift-off, beyond the take-off strip, ends the flight with "On the grass". The drawn take-off strip is now 1,000 units on levels 1–4.
- **Teaching the new skill:** a fifth quick-tour step on the landing lights, intro page 2 explains the lights, the zone and the five checks, and the level text shows the runway length.
- **Results:** the "fastest time" line is removed because time no longer counts. `par` stays in the level data for a future time challenge.

### What's new in v10 (landing is now a skill)
- **A real landing runway on every level:** a threshold, a touchdown zone, a hatched overrun cushion and an end sign. The take-off strip is separate. Touching down before the runway ends the flight with "Landed short", and touching down beyond the end ends it with "Landed too far". Rolling past the end ends it with "Off the end".
- **Glide-path lights (PAPI):** four lights beside the runway and in a box in the view. More white means you are too high and more red means too low. Two white and two red is the 3.5° path.
- **Five star checks:** gentle touchdown, touchdown zone, nose angle, stopped on the runway, and no stall. 3 stars need all of them, 2 stars allow one miss, and a win is always at least 1 star. Old saved star totals were reset because the rules changed. Best touchdown and time were kept.
- **Debrief that quotes your flight:** lift at touchdown, flare timing, thrust at touchdown, glide angle at 100 ft, and how long thrust stayed on after touchdown.
- **Fixes:** the doubled flare text, the Level 5 false "ran out of runway" after a lift-off, the Thrust meter now explains its 150% scale, the Home link hides when it would point at the current page, and the fonts are bundled so the game works offline.
- Landing data is recorded every 0.05 s near the ground (every 0.25 s otherwise).
- Runway length is in `LEVELS[...].land.len`. The glide angle is `GS`. The runway position is set at run time (see v11).

### What's new in v9
- **Bug fix:** after landing, "Try again" then Right Arrow used to reopen the result panel. Cause: the result-panel page flag (`endOpen`) and a pending result timer survived the restart, and the panel's ←/→ paging handler stayed active. `startFlight()` now cancels the timer, clears the flag, resets keys and held buttons, closes the panel and focuses the game canvas. Arrow keys page the panel only while it is open.
- **Layout:** the Force Meters panel lines up with the game view (also in fullscreen); the view grows to fill the space at 16:9; readouts are a 2×2 grid; the coaching message appears once.
- **Keys card**, R restart, P/Space pause, first-time quick tour (saved in the browser, re-open from Settings), live checklist with animation, force tips on hover/tap, Climbing/Level/Sinking label and "too steep" warning, 3-star results with replay and flight path, best score per level, larger touch buttons.

### Controls
- **Keyboard:** arrows or WASD (thrust / pitch), `Z` idle, `X` full, `P`/Space pause, `M` slow motion, `F` fullscreen, `V` advanced info, `O` settings, `H` shortcut list, `R` restart, `1`–`5` levels. Every key can be rebound in Settings → Controls.
- **Touch:** hold `+` `−` for thrust, `▲` `▼` for pitch, tap `IDLE` / `FULL`. Holding repeats.

### Layouts (chosen automatically)
| Layout | When | What you get |
|---|---|---|
| desktop | mouse / large screens | flight view + side panel + sliders |
| cockpit | touch screen, landscape, height ≤ 540 px | flight view fills the screen, thrust buttons left, pitch buttons right, ☰ menu, tap the force strip for details |
| portrait | touch screen, upright, width ≤ 700 px | view on top, force strip, one-line coaching, big thumb buttons at the bottom |

Add `?layout=cockpit`, `?layout=portrait` or `?layout=desktop` to the URL to force one (useful for testing).

On phones the full meters, level info, mission steps and the full coaching text live in the **details sheet** (tap the force strip or ☰ → Flight details). The game pauses while the sheet or the menu is open.

### Fullscreen on desktop
The flight view grows to the largest 16:9 size that fits, with the thrust/pitch controls compactly underneath and the force panel beside it. The canvas resolution follows the displayed size (and the screen's pixel ratio), so it stays sharp at any size. If the browser refuses real fullscreen, the same layout fills the window.

### Settings
Settings → **Basics** has the six things most people need (level, slow motion, advanced info, text size, theme, volume). Other tabs hold the rest. Everything is saved in the browser (`localStorage`).

### Accessibility
Colour-blind palette (Okabe-Ito), pattern fills and text labels so the forces never rely on colour alone, screen-reader live region for coaching, reduce-motion support (also disables vibration), high-contrast theme, readable-font option, strong focus outlines, focus trapping in dialogs, 44 px touch targets.

## Code map (all inside `flying-game.html`)
- `PHYSICS`: constants at the top of the script and `step(dt)`; fixed 1/60 s step. Unchanged in this version.
- `METER_DEFS` + `buildMeters()`: one template that builds both the side-panel meters and the phone force strip.
- `computeCoach()`: coaching message with full text, a short phone text and touch-specific wording.
- `applyLayout()`, `openSheet()`, `openMenu()`: phone layouts.
- `loop()`: draws only when something is moving or something changed (`markDirty()`), and pauses when the tab is hidden.
- `SCHEMA`: the Settings dialog is generated from this table.

## Notes
- Fonts (Patrick Hand, Atkinson Hyperlegible; SIL Open Font License) are bundled inside `flying-game.html`, so the game works fully offline. This makes the file about 250 KB.
- The intro is shown on the first visit only. Settings → Basics → *Show intro again* (or key `I`) brings it back. Clear site data to see it as a new player.
