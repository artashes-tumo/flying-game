# Flight School – "The 4 Forces Game"

The whole game is one file, `index.html`. Open it in a browser (double-click). It needs no server, no build step and no internet: the fonts (Patrick Hand, Atkinson Hyperlegible; SIL Open Font License) are bundled inside the file, and every picture is drawn in code (canvas and inline SVG). There are no image files and no libraries.

Take off, climb, land softly on the runway and stop. Every scenario teaches one idea about the four forces: lift, weight, thrust and drag.

## What's new: two more camera views

- **Cockpit (challenge view).** You fly from inside the plane. It is marked "challenge" in the camera list and in Settings, because you cannot see the plane from outside. Only the picture changes; the physics are the same.
  - **Through the window:** sky and ground meet at a horizon that moves down when the nose goes up, by exactly the same nose angle the side view shows. The runway is drawn in perspective from the real distance and height: small and narrow far away, wide when you are close and low, with edge lines, centre-line dashes, threshold bars, touchdown-zone and aim-point marks, and edge, threshold and end lights at dusk and night. The glide-path lights stand beside the aim point, and the glide-path box still shows. Each location keeps its look (grass, coast, mountain, island, the carrier on the sea), clouds come towards you, hills and ridges rise ahead, and on the ground the runway fills the lower view and its lines rush towards you. Gusts shake the view a little and a stall tilts it; with Reduce motion there is no shaking, only small smooth movements.
  - **Instrument panel:** airspeed, artificial horizon (with the pitch), altimeter (with an amber mark at the target height) and climb rate, each with a large readout, plus the four force meters with the same colours, patterns, F1–F4 badges and 0–200% scale as the side panel. Point at or tap a meter for its tip. A STALL light on the glare shield turns amber when the nose is too steep and blinks red in a stall; the warning sound is unchanged. On phones the panel stays clear of the on-screen buttons and switches to two rows (dials on top, meters below) when one row does not fit. The instruments shrink first; the force meters are never hidden.
  - Lesson steps that point at the plane switch to Chase for that step, and the touchdown replay is always shown from the side.
- **Flight path.** The whole flight in one zoomed-out picture: the take-off strip, the target height, the landing runway (a dashed outline shows where it will appear before you reach the target), hills, the ideal 3.5° glide path (dashed) and your own path so far (dotted). The plane is small but its force arrows are drawn big enough to read, and scale bars show distance (for example "1 km") and height (for example "500 ft"). The scales grow smoothly as the flight gets longer.
- Switching to or from these views cross-fades (instantly with Reduce motion). The canvas's screen-reader label describes the current kind of view.

## What's new in v12

- **Better graphics, same notebook look.** Ink outlines, pastel fills and the Patrick Hand font stay. New: soft shading on clouds, hills and the plane; four cloud shapes at two depths; a haze near the horizon; ground and water that get lighter towards the horizon, with water glints; runways with edge lines, a centre line and worn tyre marks in the touchdown zone; a plane shadow that shrinks and fades with height; tyre smoke, dust or spray on touchdown; a blur disc on the propeller at high thrust; a sun glow by day, a warm horizon at dusk and a moon halo at night. Expensive parts (sky, clouds, hill layers, the plane's body, the shadow) are drawn once into sprite canvases.
- **A realistic plane.** The cartoon airliner is now a high-wing, single-engine trainer seen from the side: wing with a strut, cabin windows, cowling with spinner and propeller, fin and rudder, tailplane with an elevator, and fixed landing gear with wheel fairings. The plane's height on screen comes from its lowest wheel at the current pitch, so the wheels sit exactly on the runway when the physics says you are on the ground, also while rotating and flaring. The elevator tilts with your pitch input. At dusk and night the beacon and the wing-tip strobe blink and the nav lights glow. The warm-up picture uses the same drawing.
- **Camera views.** Press `C` (or the 🎥 button, or ☰ → 🎥 on phones, or Settings → Display → Camera view) to switch between the views below (since then also **Cockpit (challenge)** and **Flight path**, see above):
  - **Chase**: the classic view (default).
  - **Wide**: zoomed out, with the 3.5° glide path drawn back from the aim point, so you see where you are going.
  - **Close-up**: zoomed in on the plane, so the force arrows are big. Good for learning.
  - **Runway cam**: fixed beside the runway threshold while you come in and land, then it follows the plane again.
  - **Automatic**: Chase, then Wide on the approach, then the runway cam close to the ground.
  The choice is saved. Views glide into each other (instantly with Reduce motion). Labels, the force arrows and the glide-path box keep a readable size at every zoom, and the force tips still work when you point at the arrows.
- **Lessons.** A new "Lessons" section at the top of the map has seven short, guided lessons: The four forces · Thrust and taking off · Pitch, lift and stall · Climbing and levelling off · Reading the glide-path lights · Flare and touchdown · Braking. Each step shows one instruction, rings the control or meter to use, and waits until you actually do it (some steps run in slow motion, explanations wait for **Next**). Every step can be skipped and every lesson can be ended. Lessons give no stars and do not change unlocks; a finished lesson gets a ✓ on the map. New players are offered Lesson 1 after the intro. Steps are read out to screen readers.
- **Flight charts need Advanced info.** Page 2 of the result screen keeps the stat boxes, but the Lift vs Weight and Thrust vs Drag charts and the data table only appear with Advanced info on. Otherwise it says: "Turn on Advanced info in Settings (or press V) to see the flight charts." Turning Advanced info on while page 2 is open draws the charts straight away. The "Read the charts" achievement now counts only results where the charts were really shown.

## Scenarios and modes

- **24 scenarios in 4 locations**: Grass strip, Coast (opens at 10 ★), Mountain (24 ★) and Island (40 ★). Each scenario opens when you have at least 1 star on the one before it. Teacher mode on the map opens everything.
- **Five star checks** per scenario (gentle touchdown, touchdown zone, nose angle, stop on the runway, no stall, or a scenario goal). 3 stars need all five, 2 stars allow one miss.
- **Daily approach** (one try a day, same air for everyone on that date), **Endless landings**, and **15 achievements**. All saved in this browser only.

## Controls

- **Keyboard:** arrows or WASD (thrust / pitch), `Z` idle, `X` full thrust, `P` or Space pause, `M` slow motion, `C` next camera view (Chase → Wide → Close-up → Runway cam → Cockpit (challenge) → Flight path → Automatic), `F` fullscreen, `V` advanced info, `O` settings, `H` or `?` keyboard shortcuts, `I` intro, `G` map, `[` / `]` previous / next scenario, `R` restart (during a lesson: restart the lesson). Every key can be changed in Settings → Controls.
- **Touch:** hold `+` `−` for thrust, `▲` `▼` for pitch, tap `IDLE` / `FULL`. Holding repeats. Tap a force arrow (or a force meter in the cockpit view) for a tip. ☰ → 🎥 changes the camera view.

## Layouts (chosen automatically)

| Layout | When | What you get |
|---|---|---|
| desktop | mouse / large screens | flight view + side panel + sliders |
| cockpit | touch screen, landscape, height ≤ 540 px | flight view fills the screen, thrust buttons left, pitch buttons right, ☰ menu, tap the force strip for details |
| portrait | touch screen, upright, width ≤ 700 px | view on top, force strip, one-line coaching, big thumb buttons at the bottom |

Add `?layout=cockpit`, `?layout=portrait` or `?layout=desktop` to the address to force one (useful for testing). On phones the full meters, the scenario text and the coaching text are in the details sheet (tap the force strip or ☰ → Flight details). The game pauses while the sheet or the menu is open.

**Fullscreen on desktop:** the flight view grows to the largest 16:9 size that fits. The canvas resolution follows the shown size and the screen's pixel ratio (capped on touch screens), so it stays sharp.

## Settings

Settings → **Basics** has the things most people need (scenario, slow motion, advanced info, text size, theme, volume). The other tabs hold the rest; the camera view is under **Display**. Everything is saved in the browser (`localStorage`: `flightSchoolSettings3` for settings, `flightSchoolProgress3` for stars, achievements and finished lessons).

## Accessibility

Colour-blind palette (Okabe-Ito), pattern fills and text labels so the forces never rely on colour alone, a screen-reader live region for coaching and lesson steps, Reduce motion (also stops vibration, touchdown dust, blinking lights and camera glides), a high-contrast theme, an easier-to-read font, strong focus outlines, focus trapping in dialogs, 44 px touch targets.

## Code map (all inside `index.html`)

- **Physics:** constants at the top of the script and `step(dt)`, fixed 1/60 s step. Unchanged in v12.
- **Scenarios:** `RAW` (data) → `makeScn()` → `SCN` / `SBY`. Per-goal checks live in `OBJ`.
- **Lessons:** `LESSON_RAW` (data, same fields as `RAW` plus `steps`) → `LESSONS` / `LBY`. The runner is `startLesson()`, `lessonNext()`, `lessonTick()`, `lessonFinish()`; the map section is `lessonsHTML()`.
- **Drawing:** `draw()` picks a renderer by `viewKind()`: `drawSideView()` (chase, wide, close-up, runway cam: a world pass through the camera), `drawCockpitView()` or `drawPathView()`, then a shared screen pass for labels, the glide-path box, the force arrows (`drawForceArrows()`), `HIT` (tooltip boxes) and messages. `startFade()` / `drawFade()` cross-fade between renderers. Scenery: `buildSky()`, `buildClouds()`, `buildLayers()` / `drawLayerShapes()`, `drawGround()`, `drawRunwaySurface()`, `drawShadow()`, `spawnPuff()`.
- **Camera:** `CAMS` / `CAMNAME` (the view list), `CAM` (zoom `z`, offset `tx`/`ty`), `camFor()` (each side view), `camResolve()` (runway cam, Automatic, and when the cockpit or flight path falls back to Chase), `camUpdate()` (blending), `VB` (the visible part of the world). The choice is `ST.camera`, saved with the other settings.
- **Cockpit view:** `ckProj()` (eye-point projection), `ckQuad()` / `ckDot()` (runway patches and lights), `cockpitGeom()` (panel layout for the layout and text size), `buildCockpitSprite()` (frame, panel and dial faces, drawn once), `drawInstruments()` (needles, horizon, readouts, meters, stall light).
- **Flight path view:** `drawPathView()` with its own scales (`PV`).
- **Plane:** `PLANE_DEF` (one list of parts for both the canvas sprite and the warm-up SVG `#plane`), `buildPlaneSprite()`, `drawPlane()`, `wheelDrop()` (wheel contact at any pitch). The force arrows start at `ARROW_UP`, `ARROW_DN`, `ARROW_FWD` from the plane's centre.
- **Settings:** `SCHEMA` builds the Settings dialog, `ACTIONS` the rebindable keys.
- **Results:** `showEnd()`, `renderEnd()`, `endDataHTML()` / `flightSection()` (charts only with Advanced info).
- **Loop:** `loop()` draws only when something moves or changed (`markDirty()`), and pauses when the tab is hidden.

## Test checklist

Open `index.html`. Do the list on desktop, then again with `?layout=cockpit` and `?layout=portrait` (in the browser's device toolbar).

1. **Every view, every layout.** Start 1.1 and press `C` seven times: Wide → Close-up → Runway cam → Cockpit (challenge) → Flight path → Automatic → Chase. The 🎥 button name changes each time, side views slide and the cockpit / flight path fade in, and a "CAMERA: …" label shows. Point at (or tap) each force arrow, and in the cockpit each force meter: the tip appears. Repeat with `?layout=cockpit` (the panel stays clear of the side buttons; ☰ → 🎥) and `?layout=portrait` (two rows of instruments, all four meters visible).
2. **Full flight on 1.1 in the cockpit view.** On the runway the lines rush towards you. Rotate: the horizon drops as the nose rises, and the artificial horizon matches. Climb to 1,000 ft (amber mark on the altimeter), level off, watch the runway grow from a small trapezoid, use the glide-path lights beside it, flare, land, stop. Then ▶ Replay touchdown: it plays from the side.
3. **Gusts and wind (2.2 Bumpy air, 3.4 Valley gusts or 4.4 Storm front) in the cockpit view.** The view shakes a little in gusts; push the nose past 15° up high: the view tilts, the STALL light blinks red and the warning sounds.
4. **Night landing (4.2).** Edge lights, green threshold, red end, glide-path lights and stars from the cockpit; also in the flight path view.
5. **Carrier landing (4.3 or 4.6).** In the cockpit the deck and the ship's tower sit on the sea and move away from you; in the runway cam the camera moves with the ship.
6. **Mountain with a ridge (3.2 Ridge climb, 3.3 Over the hill).** The ridge rises ahead in the cockpit with its height label; in the flight path view it is a labelled triangle under your dotted path.
7. **Flight path view on a long approach (4.5 Last drop of fuel, or Lesson 1).** The dashed ideal glide path, your dotted path, the runway, and the distance and height scale bars; the scales grow smoothly. On 1.1 before the target height the runway is a dashed outline.
8. **Lessons.** Play a lesson in the cockpit view: steps about the plane switch to Chase and back; the ring still marks the controls and meters.
9. **Reduce motion on** (Settings → Sound & access): views switch instantly, the cockpit does not shake (only a small smooth bob and tilt), the STALL light stays on instead of blinking, no touchdown dust.
10. **Page 2 of the result screen.** With Advanced info off: only the stat boxes and the "Turn on Advanced info…" line. Press `V`: the charts appear.
11. **Themes.** Dark, then High contrast, then the colour-blind colours: check the cockpit panel, the meters' patterns and the flight path view in each.

## Earlier versions

- **v11:** the landing runway is placed when you reach the target height (`placeRunway()`); missed approach result; landing on the grass after take-off ends the flight; a fifth quick-tour step on the landing lights.
- **v10:** a real landing runway with threshold, touchdown zone and overrun; glide-path lights (PAPI); five star checks; a debrief that quotes your flight.
- **v9:** keys card, quick tour, live checklist, force tips, 3-star results with replay and flight path, larger touch buttons.
