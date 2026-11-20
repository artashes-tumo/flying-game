# Flight School – "The 4 Forces Game"

The whole game is one file, `index.html`. Open it in a browser (double-click). It needs no server, no build step and no internet: the fonts (Patrick Hand, Atkinson Hyperlegible; SIL Open Font License) are bundled inside the file, and every picture is drawn in code (canvas and inline SVG). There are no image files and no libraries.

Take off, climb, land softly on the runway and stop. Every scenario teaches one idea about the four forces: lift, weight, thrust and drag.

## What's new: notifications, smooth panels, tags and a new briefing

- **Notifications:** a new achievement, rank, location, plane colour or pilot item shows a small card at the top centre (it slides down, stays about 4 s, then slides up) with a short chime. Several show one after another. Hover pauses it, clicking opens the achievements list with that one highlighted, × closes it. During a flight it is smaller and never covers the phone HUD or pauses the game. With Reduce motion it only fades.
- **Smooth panels:** Settings slide in from the right, the pause menu fades in with a slight zoom while the flight dims, the Hangar and the achievements slide in, the briefing, results and licence card rise up, menu screens slide forward and back, and tab contents cross-fade. Reduce motion: very short fades only.
- **Centred screens:** How to play, the level select and the location screens sit in the middle; tall content scrolls inside the box. Daily approach and Endless landings are a centred pair.
- **Condition tags:** each scenario card shows coloured tags (🌬 Wind, 〰 Gusts, ↯ Shear, 🌙 Night, 🌅 Dusk, ⚖ Heavy, ⚠ Engine out, ⛽ Little fuel, ⚓ Carrier, ✈ a plane other than the Trainer), always with an icon and a word. Hover for the meaning; ⓘ Icon key lists them all.
- **Briefing in sections:** header with stars and tags, Your goal (the steps), Conditions (one row each, at your explanation level), You will learn (with the star checks folded away), Plane, and Fly this scenario. Fits one screen on desktop and on a phone held sideways.

## What's new: compact pause menu and Hangar, automatic touch / keyboard

- **Pause menu:** a small card over the dimmed flight: **▶ Continue** (focused), **↺ Restart**, and one row with 🔈 mute, the volume slider, ⚙ (Quick settings as a second small card on top: all quick options, More settings, Level select) and ⌂ (main menu, asks "Leave this flight?" first). A stall pause shows one short line above. Esc, P, the fullscreen double-Esc and the auto-pauses work as before; Esc closes the ⚙ card first.
- **Hangar on one screen:** a big preview on top (plane with its comparison bars, or the pilot with name, 🎲 Random, ↺ Reset, 🪪 licence and the faces), then horizontal rows: the planes and the paints, or the pilot groups (Skin, Hair, Face, Headgear, Jacket) and their choices. Rows scroll by swipe, mouse wheel or trackpad, with ← → between items and small ‹ › buttons on mouse devices. Locked items keep a small 🔒 with the requirement in the tooltip. Fits without vertical scrolling on desktop and on a phone held sideways.
- **Achievements** moved to the main menu (🏆 with the count).
- **Touch or keyboard, automatically:** the game looks at how you play, not at the device name. On touch the keyboard guide (KEYS panel), key hints, the keyboard part of How to play → Controls and key re-binding in Settings are hidden, and coach messages, lessons and the tour talk about the on-screen buttons. The first real key press switches to keyboard hints; a touch after 20 s without keys switches back. Touch screens keep the ❚❚ pause button, also with a keyboard. Phones pick the sideways (cockpit) or upright (portrait) layout and switch when rotated, without restarting the flight; `?layout=` still forces one.

## What's new: explanation levels

- **Three levels** change how the game talks, never the physics, difficulty, star checks or scoring, so stars stay fair:
  - **Explorer** (about 6 to 10): short everyday sentences, no units or numbers. Speed and height as words ("fast", "up high"), climb as an arrow ("↑ going up"), the forces as pushes and pulls ("Lift is winning!"). No percentages on the meters or the arrows.
  - **Student** (about 11 to 16): the game as before: %, ft, kt, fpm, "Lift > Weight, so you climb".
  - **Pilot** (16 and up, university): real terms and physics: angle of attack, lift coefficient C_L (shown next to the pitch), sink rate, glide ratio, L/W, lift = ½ ρ v² S C_L, ground effect. Results add "The numbers" (sink rate, airspeed, pitch, L/W at touchdown, flare timing, approach angle against the ideal path, and one tip from them). Lessons add a short "The physics" box. Pilot can switch to metric units (Settings → Display → Units: km/h, m, m/s).
- The age ranges only pick the explanation level; the age itself is never saved.
- **Choosing:** on the first visit (and once for older saves) the game first says hi ("Hi, welcome to Flight School!"), then asks "How old are you?" with three buttons: 6 to 10 (Explorer), 11 to 15 (Student), 16 or older (Pilot). "Rather not say" or Skip keeps Student. Only the level is saved, never the age. Change it any time in Quick settings (also in the pause menu); mid-flight the texts change at once. Choosing Explorer turns Advanced info off and Pilot turns it on (you can still change it).
- Safety messages (stall, too fast, too low, hill, runway ending) stay just as short and urgent at every level.

## What's new: a living main menu

- **The scene:** behind the main menu flies a small free-flight sky made from the game's own scenery (hills, trees, runway, sea, mountains, islands) in slow parallax. Every 40–60 s it cross-fades to another location you have unlocked (a first visit shows only the Grass strip). The time of day follows your clock: day, dusk, or night with stars, a moon and runway lights. Small life: birds, a windsock, a balloon (or a glider at dusk and night) far away, boats at the coast and the island, and now and then another Hangar plane in the distance.
- **Readable:** the title and buttons sit on a soft paper panel in every theme (fully solid in high contrast).
- **Fly it:** your plane, paint and pilot cruise in gentle waves. Hold the mouse on the empty sky and move up / down, drag on a touch screen, or use ↑ ↓ (pitch) and ← → (speed) when no button is focused. It cannot stall or crash, is pushed back gently from the top and the ground, and loops are allowed. Small force arrows show while you steer. A hint at the bottom ("Drag the sky (or use ↑ ↓) to fly") fades after the first time and is remembered. After 5 s without input the plane flies itself again; Tab or a focused button hands the arrows back to the buttons (arrows then move between the menu buttons). The glider flies silently, the fast jet a bit quicker; other planes hum softly at a low volume that follows the effects volume.
- **Reduce motion:** a still scene and a still plane, no steering. The animation runs only while the main menu is visible and stops in flights and when the tab is hidden.

## What's new: menus, How to play, Quick settings and the pause menu

- **Main menu first, every time.** A big FLIGHT SCHOOL title over a calm sky where your plane (with its paint and pilot) drifts by; with Reduce motion it is a still picture. Menu music plays. Buttons: **▶ PLAY**, **Continue: <last scenario>** (once you have flown; opens its briefing), **Pilot** and **Plane** (the Hangar on that tab), **How to play**, **Settings** (opens on the Quick tab). The licence badge in the corner (face, name, rank, stars) opens the licence card. On a first visit How to play pulses gently with "New here? Start here!"; nothing pops up and PLAY works straight away.
- **Level select** (after PLAY): four location cards with a small drawing of each place, its tagline, stars earned of the total, and "Opens at X stars" with a lock while closed (clicking a closed one says how many stars you need). Below: **Daily approach** and **Endless landings** (same rules as before: one daily try, streaks, best runs). **Achievements** are on the main menu (🏆 7/15).
- **A location's scenarios:** its drawing and name, then one card per scenario: number and name, stars or "not flown yet", a lock with what opens it, and icons for the conditions (🌬 wind, 〰 gusts, ↯ wind shear, 🌙 night, 🌅 dusk, ⚖ heavy, ⚠ engine failure, ⛽ little fuel, ⚓ carrier) plus the suggested plane. An open card opens the briefing card ("Fly this scenario", "Change plane").
- **How to play** has six tabs: Four forces · Warm-up (the force-matching game, right there) · Lessons (✓ = done) · Controls (your current keys, and touch) · Landing guide (glide-path lights, touchdown zone, flare, the five star checks) · Quick tour (replay it). It remembers the tab you were on. The old intro pop-up is gone; Settings → Game → "Open How to play" and the intro key `I` open this screen.
- **Moving around:** every screen has a Back button and `Esc` goes back one screen (on the main menu it does nothing, except leave fullscreen). In menus Esc never pauses. Screens slide in; with Reduce motion they switch instantly. `M` opens the level select (during a flight the flight waits paused underneath, and Back returns to it).
- **Quick settings:** Advanced info, Coaching tips, Slow motion, Camera view, Volume, Music on/off, Sound effects on/off (warnings stay on), Text size and Theme. It is Settings → Quick and is also built into the pause menu (the same panel). Restart-needed options (turbulence, fuel burn, stall protection) stay in Settings → Game. Teacher mode moved to Settings → Game.
- **Pause menu:** whenever a flight is paused (Esc, P, ❚❚, the touch ❚❚ button in the top corner of the flight view, auto-pause on a stall, the tab hidden, fullscreen ended): ▶ Continue (focused), ↺ Restart, Quick settings, ⚙ More settings, 🗺 Level select and ⌂ Main menu (click twice: the flight is lost). The flight stays visible, dimmed; thrust and pitch do nothing while it is open. A stall pause shows its explanation at the top. In fullscreen the first Esc opens it and the second leaves fullscreen with the menu still open. A desktop app can set `window.flightSchoolHost = {quit: function(){…}}` to add a "Quit game" button.
- **Results:** Next scenario stays; "Map" is now **Level select** (that location's scenarios), plus **Main menu**.
- **Saved:** the last scenario (for Continue), the last location and the last How-to-play tab (`flightSchoolMenu`). Old saves keep all stars, unlocks, lessons, achievements, daily streak, endless best, plane and pilot.

## What's new: your own pilot

- **Pilot creator:** the Hangar (`G`) has a second tab, **Pilot**. A big live preview (try its faces: calm, happy, very happy, worried, shocked) and five groups: **Skin** (8 tones), **Hair** (9 styles: short, buzz cut, long, curly, afro, ponytail, bun, braids, bald; 8 colours, natural and fun), **Face** (eyes, eyebrows, mouth; freckles, beard, moustache, glasses), **Headgear** (none, headset, cap, aviator helmet with goggles, captain's hat) and **Jacket** (8 colours, golden wings badge). Hair is drawn to fit under every headgear (a ponytail or bun peeks out under a cap, nothing pokes through the helmet). **🎲 Random** and **↺ Reset** (the name stays). There is no gender switch: every option goes with every other one.
- **Name:** up to 16 letters, numbers and spaces, default "Pilot". It is kept only in this browser.
- **Only for fun:** the pilot never changes how a plane flies, the stars or the difficulty.
- **Unlocks:** most items are free. The aviator helmet opens after 1.8 Silent wings and 3.7 Ridge glider (the glider scenarios), the gold jacket at ★ 30, the captain's hat at ★ 55, the golden wings badge with the "Every star" achievement. Locked items are dashed and say what opens them (Teacher mode opens everything).
- **In the plane:** the pilot sits in front of the seat, behind the glass, in every plane (head and shoulders over the rim of the Biplane's open cockpit). The face reacts: worried in a stall warning, shocked in a stall or a crash (a little shake, none with Reduce motion), very happy after a soft landing.
- **Briefing and results:** the briefing says "Captain <name>, ready for take-off?". The results show the pilot's face (very happy for a butter landing or 3 stars, happy for a normal landing, worried for a hard landing, shocked for a crash) and the name: "<name> touched down at 140 fpm".
- **Pilot licence card:** from the Pilot tab (🪪 Licence card) and from the main menu (the licence badge): face, name, rank, total stars, softest touchdown, number of flights, favourite plane (the one flown most) and achievements.
- **Ranks** by stars: Student pilot (0), Private pilot (★ 10), Commercial pilot (★ 30), Captain (★ 55), Ace (★ 80, of 87). A new rank is celebrated on the results screen.
- **Saving:** the pilot is saved with your progress. An older save gets the default pilot and is asked once, gently, whether to make its own ("Maybe later" skips). Settings → Reset level progress clears the stars as before, then asks separately about the pilot: it is kept unless you choose "Reset the pilot too".

## What's new: redrawn planes

- **Every plane redrawn as a true side view**, matching the camera: wings seen edge-on as a thin airfoil (with the darker far wing just peeking out), real proportions, and the same ink lines and soft shading as the Trainer. New details: panel lines, door outlines, hinge lines, antennas, registration letters (FS-101, FS-G7, FS-C30, FS-B2, FS-J9) and an empty seat behind see-through cockpit glass, ready for a pilot.
  - **Glider:** slim pod and tail boom, big bubble canopy, shoulder wing, T-tail, one main wheel and a tail skid (it rests on the skid when stopped).
  - **Cargo plane:** big round body, high wing, two turboprops (the far one partly hidden), cabin portholes, rear ramp, tall tail, tandem main wheels.
  - **Biplane:** staggered wings with struts and wires, open cockpit, round engine with cylinders, tail wheel.
  - **Fast jet:** slim pointed body, low swept wing, tandem bubble canopy, intake, jet nozzle with heat shimmer at high thrust (none with Reduce motion), and **gear that folds up after take-off and comes down for the approach**.
- The same drawing is used everywhere: in flight, the touchdown replay, the flight-path view, the Hangar cards, the briefing card, the result screen ("Flown with the …") and the warm-up.

## What's new: the Hangar and five planes

- **The Hangar** (toolbar or ☰ → ✈ Hangar, the map, "Change plane" on a briefing card, or `G`) is where you pick your plane and its paint. It has tabs; today there is one, **Plane** (a Pilot tab can be added later in the same place).
- **Five planes**, each teaching one idea. Every card shows the plane in its paint, what it teaches, and bars that compare it with the Trainer (lift, drag, engine, weight, speed, stall safety) with numbers and words:
  - **Trainer:** the plane you know: balanced and forgiving. It flies exactly as before.
  - **Glider:** no engine (thrust stays at 0, like an engine failure), long wings, very little drag, light. You can fly without thrust if you trade height for speed. Only for scenarios that start in the air.
  - **Cargo plane:** heavy twin with strong engines: a long take-off run, a higher lift-off speed, a nose that answers slowly, and a gentle stall. More weight needs more lift.
  - **Biplane:** two wings, lots of lift and lots of drag: a very short take-off, a slow top speed and a very forgiving stall (18°).
  - **Fast jet:** small swept wings, a strong jet and little drag: fast, stalls early (12°) and lands fast.
- **Paints:** seven per plane (body and stripe colour). Some open with stars (6, 15 or 30) or the Butter achievement; locked ones say what they need. The outlines stay ink, so the force arrows and labels stay readable.
- **Planes and scenarios:** every scenario suggests a plane (the Trainer for most). The briefing shows the suggested plane and the plane you will fly. Stars, best results and achievements count only with the suggested plane; with another plane the result says "Practice flight: stars only with the suggested plane". A plane that cannot do a scenario shows why (for example the Glider: "Needs an approach start"; the Cargo plane: "Take-off strip too short") and you fly the suggested plane there. These limits come from test flights of every plane on every scenario. Lessons always use the Trainer; the daily approach and endless mode use the suggested plane.
- **New scenarios:** 1.7 *Biplane hop* (short grass strip), 1.8 *Silent wings* (glider, long glide), 2.7 *Heavy hauler* (cargo plane, long runway), 2.8 *Fast arrival* (fast jet approach), 3.7 *Ridge glider* (glider over a ridge to the mountain strip).
- Coach messages, tips, the debrief, the intro, the quick tour and the lift-vs-pitch chart use the flying plane's real numbers (stall angle, rotate angle, best glide, lift-off speeds). The cockpit view has a frame and gauges per plane: a canopy and no engine gauge in the glider, a canopy and an N1 / EGT gauge in the jet, an open cockpit under the top wing in the biplane, a wide windshield and twin RPM in the cargo plane.

## What's new: keys and the fullscreen button

- **Fullscreen** moved from the toolbar and the ☰ menu to a small icon button in the top-right corner of the flight view (corners point out; in fullscreen they point in). It stays clear of the HUD, the force meters and the coaching messages in every layout, and is hidden when the browser has no fullscreen. Esc in fullscreen: see *Fullscreen* below.
- **New keys:** `Esc` pauses and resumes (it still closes an open panel first), `P` stays as a second pause key, Space no longer pauses. `S` opens and closes Settings (`O` still works), `M` opens and closes the map (G is gone), slow motion moved from M to `T`. Because S used to be "nose down", the second nose-down key is now `Q`.
- **Saved keys are moved over once:** only the old defaults change (Space is taken off pause, Esc added; G → M; M → T; S → Q and S → Settings). A key you chose yourself stays, and a new key is only given if no other action uses it, so no key ends up on two actions.

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
- **Lessons.** A "Lessons" tab in How to play has seven short, guided lessons: The four forces · Thrust and taking off · Pitch, lift and stall · Climbing and levelling off · Reading the glide-path lights · Flare and touchdown · Braking. Each step shows one instruction, rings the control or meter to use, and waits until you actually do it (some steps run in slow motion, explanations wait for **Next**). Every step can be skipped and every lesson can be ended. Lessons give no stars and do not change unlocks; a finished lesson gets a ✓ on the map. New players are offered Lesson 1 after the intro. Steps are read out to screen readers.
- **Flight charts need Advanced info.** Page 2 of the result screen keeps the stat boxes, but the Lift vs Weight and Thrust vs Drag charts and the data table only appear with Advanced info on. Otherwise it says: "Turn on Advanced info in Settings (or press V) to see the flight charts." Turning Advanced info on while page 2 is open draws the charts straight away. The "Read the charts" achievement now counts only results where the charts were really shown.

## Scenarios and modes

- **29 scenarios in 4 locations**: Grass strip (8), Coast (8, opens at 10 ★), Mountain (7, opens at 24 ★) and Island (6, opens at 40 ★): 87 stars in all. Each scenario opens when you have at least 1 star on the one before it. Teacher mode (Settings → Game) opens everything. The unlock thresholds did not change, so old saves keep every location they had open.
- **Five star checks** per scenario (gentle touchdown, touchdown zone, nose angle, stop on the runway, no stall, or a scenario goal). 3 stars need all five, 2 stars allow one miss.
- **Daily approach** (one try a day, same air for everyone on that date), **Endless landings**, and **15 achievements**. All saved in this browser only.

## Controls

- **Keyboard:** arrows (thrust ← →, pitch ↑ ↓), or `A` / `D` for thrust and `W` / `Q` for nose up / down; `Z` idle, `X` full thrust; `Esc` pause and resume (if a panel is open, Esc closes it first; `P` also pauses and resumes); `S` (or `O`) settings, open / close; `M` level select, open / close; `G` Hangar, open / close; `T` slow motion; `C` next camera view (Chase → Wide → Close-up → Runway cam → Cockpit (challenge) → Flight path → Automatic); `F` fullscreen; `V` advanced info; `H` or `?` keyboard shortcuts; `I` How to play; `[` / `]` previous / next scenario; `R` restart (during a lesson: restart the lesson). Space does not pause. Game keys do not fire while you change a key in Settings → Controls. Every key can be changed there.
- **Touch:** hold `+` `−` for thrust, `▲` `▼` for pitch, tap `IDLE` / `FULL`. Holding repeats. Tap a force arrow (or a force meter in the cockpit view) for a tip. The ❚❚ button in the top corner of the flight view opens the pause menu. ☰ → 🎥 changes the camera view. The fullscreen button is the ⤢ icon in the top-right corner of the flight view (hidden where the browser has no fullscreen, such as iPhone Safari).

## Layouts (chosen automatically)

| Layout | When | What you get |
|---|---|---|
| desktop | mouse / large screens | flight view + side panel + sliders |
| cockpit | touch screen, landscape, height ≤ 540 px | flight view fills the screen, thrust buttons left, pitch buttons right, ☰ menu, tap the force strip for details |
| portrait | touch screen, upright, width ≤ 700 px | view on top, force strip, one-line coaching, big thumb buttons at the bottom |

Add `?layout=cockpit`, `?layout=portrait` or `?layout=desktop` to the address to force one (useful for testing). On phones the full meters, the scenario text and the coaching text are in the details sheet (tap the force strip or ☰ → Flight details). The game pauses while the sheet or the menu is open.

**Fullscreen:** the ⤢ button in the top-right corner of the flight view, or `F`. On desktop the flight view grows to the largest 16:9 size that fits; the canvas resolution follows the shown size and the screen's pixel ratio (capped on touch screens), so it stays sharp.
In Chrome, Edge and Dia the game keeps Esc in fullscreen (Keyboard Lock): the first Esc pauses and shows "Press Esc again to exit fullscreen", the second Esc leaves fullscreen and the game stays paused (`P` resumes). Holding Esc down also leaves fullscreen there (the browser's own rule). In Firefox and Safari the browser leaves fullscreen on the first Esc; the flight then pauses itself, so you never lose the plane.

## Settings

Settings → **Quick** has the things most people need (advanced info, coaching tips, slow motion, camera view, volume, music and effects on/off, text size, theme); the pause menu shows the same panel. The other tabs hold the rest; the camera view is under **Display**. Everything is saved in the browser (`localStorage`: `flightSchoolSettings3` for settings, `flightSchoolProgress3` for stars, achievements and finished lessons).

## Accessibility

Colour-blind palette (Okabe-Ito), pattern fills and text labels so the forces never rely on colour alone, a screen-reader live region for coaching and lesson steps, Reduce motion (also stops vibration, touchdown dust, blinking lights and camera glides), a high-contrast theme, an easier-to-read font, strong focus outlines, focus trapping in dialogs, 44 px touch targets.

## Code map (all inside `index.html`)

- **Physics:** constants at the top of the script and `step(dt)`, fixed 1/60 s step. `step()` reads the flying plane's numbers (`PL`, made by `planePhys()` from `PLANES`); with the Trainer they are exactly the old constants.
- **Scenarios:** `RAW` (data) → `makeScn()` → `SCN` / `SBY`. `craft` is the suggested plane (Trainer when missing). Per-goal checks live in `OBJ`.
- **Lessons:** `LESSON_RAW` (data, same fields as `RAW` plus `steps`) → `LESSONS` / `LBY`. The runner is `startLesson()`, `lessonNext()`, `lessonTick()`, `lessonFinish()`; the map section is `lessonsHTML()`.
- **Drawing:** `draw()` picks a renderer by `viewKind()`: `drawSideView()` (chase, wide, close-up, runway cam: a world pass through the camera), `drawCockpitView()` or `drawPathView()`, then a shared screen pass for labels, the glide-path box, the force arrows (`drawForceArrows()`), `HIT` (tooltip boxes) and messages. `startFade()` / `drawFade()` cross-fade between renderers. Scenery: `buildSky()`, `buildClouds()`, `buildLayers()` / `drawLayerShapes()`, `drawGround()`, `drawRunwaySurface()`, `drawShadow()`, `spawnPuff()`.
- **Camera:** `CAMS` / `CAMNAME` (the view list), `CAM` (zoom `z`, offset `tx`/`ty`), `camFor()` (each side view), `camResolve()` (runway cam, Automatic, and when the cockpit or flight path falls back to Chase), `camUpdate()` (blending), `VB` (the visible part of the world). The choice is `ST.camera`, saved with the other settings.
- **Cockpit view:** `ckProj()` (eye-point projection), `ckQuad()` / `ckDot()` (runway patches and lights), `cockpitGeom()` (panel layout for the layout and text size), `buildCockpitSprite()` (frame, panel and dial faces, drawn once), `drawInstruments()` (needles, horizon, readouts, meters, stall light).
- **Flight path view:** `drawPathView()` with its own scales (`PV`).
- **Planes:** `PLANES` (data: name, texts, `phys` factors, `needs`, paints), `PAINTS`, `planePhys()`, `planeIssue()` (why a plane cannot fly a scenario), `flightPlaneId()` (which plane really flies). Looks: `LOOKS` (true side-view parts, far wing, registration, wheel contacts, arrow anchors, props or jet, retractable gear, elevator, lights, cockpit frame and engine gauge, and `pilot` = where a pilot's head goes), `drawAirframe()` + `drawLive()` (one drawing for everything), `buildPlaneSprite()`, `drawPlane()`, `planePicURL()` / `planeImg()` (the same drawing as a picture for the Hangar, briefing, results and warm-up), `wheelDrop()` (wheel contact at any pitch; the biplane and the glider sit on their tails when slow). The Hangar: `HANGAR_TABS`, `showHangar()`, `hangarPlaneHTML()`; the choice is saved under `flightSchoolHangar`.
- **Pilot:** data `PSKIN`, `PHAIR`, `PHAIRCOL`, `PEYES`, `PBROWS`, `PMOUTH`, `PEXTRA`, `PHEAD`, `PJACKET`, `PBADGE`, `PEXPR`, `PILOT_DEF`, `RANKS` (items with `req` are locked: `reqOpen()` / `reqText()`); `normPilot()` / `pilot()` / `savePilot()` (saved as `PG.pilot`); `drawPilot()` draws one at any size and expression; `pilotImg()` its picture; `drawPilotIn()` puts it in a plane at `LOOKS[...].pilot`; `pilotMood()` the face in flight. Pilot tab `hangarPilotHTML()` / `bindHangarPilot()`; licence card `showLicence()`; `pilotOffer()` (once, for older saves); `askPilotReset()` (after Reset progress).
- **Explanation levels:** the text table `TX` and `tx(key, vals)` (fallback to Student), `lvl()`, `LEVELS`, `levelOffer()`, `LESSON_LV`, `pilotNumsHTML()`, `achD()`.
- **Menu scene:** `MS`, `msBuild()`, `msLife()`, `clockTod()`, `menuLocs()`; the menu plane `MPL` with `mpStep()`, `mpDraw()`, `mpKey()`, `mpSound()`; loop `menuBgStart()` / `drawMenuBg()` / `menuBgStop()`.
- **Menus:** `SCREENS` (main, levels, loc, learn) with `showScreen()` / `screenBack()` / `closeScreens()`, `SCR_STACK` (the way back), `mainHTML()`, `levelsHTML()`, `locHTML()` (`scnCardHTML()`, `scnIcons()`), `learnHTML()` / `learnBody()` (`LEARN_TABS`), `sceneSVG()` (location drawings), `drawMenuBg()` (the moving background), `matchHTML()` / `bindMatch()` (warm-up), `MENU` saved as `flightSchoolMenu`. Pause menu: `updatePauseUI()` → `openPause()` / `renderPause()` / `closePause()`. Quick settings: `QUICK` + `quickHTML()`, one handler `settingInput()`, `syncQuick()`.
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
12. **Esc pause and resume.** While flying press `Esc`: PAUSED. Press it again: the flight goes on. `P` does the same. Space does nothing.
13. **Esc with a panel open.** Open Settings, the level select, the flight details (phones), How to play, the quick tour or a tooltip, and press `Esc`: only that panel closes, the game does not pause.
14. **S and M.** `S` opens Settings and `S` again closes it; `M` opens the level select and `M` again closes it (also from the result screen). In Settings → Controls, click a key to change it: while it says "Press a key…", S, M, T and Esc do not trigger anything (Esc just cancels).
15. **T for slow motion.** `T` turns slow motion on and off; Settings → Quick → Slow motion says "Key: T".
16. **Fullscreen in Chrome / Edge / Dia.** Click ⤢ (or press `F`), fly, press `Esc`: the game pauses and shows "Press Esc again to exit fullscreen". Press `Esc` again: fullscreen ends and the game is still paused; `P` resumes.
17. **Fullscreen in Firefox or Safari.** Enter fullscreen, fly, press `Esc`: the browser leaves fullscreen and the flight is paused.
18. **Old saved keys.** In a browser that played an older version: Space no longer pauses, M opens the level select, T is slow motion, and any key you had changed is still yours.
19. **1.1 with the Trainer** (Hangar → Trainer): take-off, climb and landing feel exactly like before: lift-off at about 150 kt after roughly 950 ft, 1,000 ft after about 25 s, stall at 15°.
20. **Each new plane on its own scenario:** 1.7 with the Biplane (lifts off within the short strip), 1.8 with the Glider (no thrust; glide at about 4°), 2.7 with the Cargo plane (long run, slow nose), 2.8 with the Fast jet (fast approach, stall light at a lower angle), 3.7 with the Glider (stay high over the ridge).
21. **Glider blocked:** pick the Glider and open 1.1: its card says "Needs an approach start", its button is disabled, and the briefing says you fly the Trainer.
22. **Practice flight:** pick the Biplane and fly 1.2: the result says "Practice flight: stars only with the suggested plane", and the level select's stars do not change.
23. **Paint unlocks:** with fewer than 6 stars the Barnstormer paint shows "★ 6 needed"; after 6 stars it can be chosen. Night owl needs the Butter achievement.
24. **The Hangar in every layout:** desktop (toolbar, `G`, the main menu, "Change plane" on a briefing), `?layout=cockpit` and `?layout=portrait` (☰ → ✈ Hangar). Tab, Shift+Tab and Esc work; a screen reader reads each bar as text.
25. **The cockpit view per plane:** Glider (canopy, four gauges, no engine), Cargo plane (wide windshield, RPM ×2), Biplane (top wing and struts overhead), Fast jet (canopy, N1 and EGT).
26. **An old save:** in a browser that played before this update, the game starts with the Trainer, all stars and unlocked locations are still there, and no key is on two actions (if G was still your map key, the Hangar key is left empty: set one in Settings → Controls).
27. **Each plane in the Hangar with every paint:** open the Hangar (`G`), pick each plane and click through its paints; the picture changes colour, the outlines stay dark. Teacher mode on the map opens the locked paints for a quick check.
28. **Take-off and landing with each plane:** 1.1 with the Trainer, Cargo plane, Biplane and Fast jet; 1.8 with the Glider (it starts in the air). The wheels touch the runway exactly at touchdown, also nose-high in the flare; the Biplane and the Glider settle onto their tails when they stop.
29. **The fast jet's gear:** fly 1.1 or 2.8 with the Fast jet: the gear folds into the body a few seconds after take-off and comes back down when the glide-path lights show up on the approach; with Reduce motion it snaps instead of swinging and there is no heat shimmer.
30. **Night lights:** fly 4.2 (night) with each plane: red nav light with a white strobe, blinking red beacon, white tail light (steady with Reduce motion).
31. **Themes:** the Hangar and the planes in flight with Dark, High contrast and the colour-blind colours: the planes keep ink outlines and the force arrows stay readable.
32. **Pilot creator, every group:** Hangar (`G`) → Pilot. Click a skin tone, each hair style and colour, eyes, eyebrows, mouth, each extra, each headgear, a jacket colour: the preview and the small pictures change at once; a screen reader says e.g. "Hair colour: dark brown"; the tooltips say the same. Arrow keys move along a row; ← → on the tab bar switch Plane / Pilot.
33. **Random and Reset:** 🎲 Random gives a new look each press (never a locked item) and keeps the name; ↺ Reset goes back to the default look.
34. **Name:** type "Ana-Maria! 2024 the great": the dash and "!" are dropped and it stops at 16 characters; Enter saves it; reload: it is still there.
35. **Every headgear with long hair** (and with ponytail, bun, afro, braids): long hair falls below a cap and the captain's hat, ponytail and bun peek out under a cap, nothing pokes through the aviator helmet.
36. **A locked item unlocking:** with no stars the aviator helmet says "🔒 Finish 1.8 Silent wings and 3.7 Ridge glider"; land 1.8 and fly 3.7 with the glider: it can be chosen. The captain's hat needs ★ 55.
37. **The pilot in every plane:** fly 1.1 with the Trainer, Cargo plane, Biplane and Fast jet and 1.8 with the Glider in the Close-up view: the head (with headgear) sits behind the glass in front of the seat; in the Biplane head and shoulders show above the open cockpit (choose the aviator helmet to see the goggles). The Hangar pictures show the pilot too.
38. **Reactions in flight:** raise the nose until the stall warning: the pilot looks worried; stall: shocked (a little shake, none with Reduce motion); a soft landing: very happy.
39. **Briefing:** open a scenario from the level select: "Captain <name>, ready for take-off?" with the pilot's face.
40. **Results:** a butter landing or 3 stars → very happy face; a firm landing → happy; a hard landing → worried; a crash → shocked. The text says "<name> touched down at … fpm".
41. **Licence card and rank-up:** open 🪪 from the Pilot tab and from the main menu badge: rank, stars, softest touchdown, flights, favourite plane, achievements. Get the 10th star: the results say "🎉 Promoted! <name> is now a Private pilot".
42. **Old save:** in a browser with stars from before this update: the default pilot flies, a card "NEW: YOUR OWN PILOT" appears once (Maybe later / Create my pilot) and never again. Settings → Game → More options → Reset level progress (click twice): stars go, the pilot stays; "Reset the pilot too" brings back the default.
43. **The Pilot tab in all three layouts** (desktop, `?layout=cockpit`, `?layout=portrait`) with Light, Dark and High contrast: every button is reachable with Tab, at least 44 px, and readable.

44. **First visit as a new player:** clear the site data and open the page: the main menu (not a flight), the plane drifting by, How to play pulsing with "New here? Start here!", no Continue button. PLAY works straight away.
45. **A returning player:** fly 1.1, reload: the main menu shows "Continue: 1.1 · First flight"; it opens that briefing card.
46. **Every main menu button:** PLAY → level select; Pilot → Hangar on Pilot; Plane → Hangar on Plane; How to play; Settings (Quick tab); the licence badge → the licence card. Each one's Back / ✕ / Esc returns to the main menu with focus on the button you used.
47. **A locked and an open location:** with few stars click Coast: "The Coast opens at 10 stars. You have …". Click Grass strip: its scenarios.
48. **A locked and an open scenario:** a locked card says "Earn at least 1 star on … first"; an open one opens the briefing; "← Grass strip" on the briefing goes back to the cards.
49. **How to play:** each tab; the Warm-up (place all four forces, ↺ Start again, ▶ Go fly); a lesson from the Lessons tab (End lesson brings you back to the Lessons tab); Controls shows your own keys; Quick tour starts a flight with the tour. Leave and come back: the same tab is open.
50. **Daily and Endless from the level select:** the daily asks for a second click and then flies (once a day); Endless starts.
51. **Esc through every screen:** main menu → PLAY → Grass strip → a briefing: Esc closes the briefing, Esc → level select, Esc → main menu, Esc does nothing more. During a flight Esc opens and closes the pause menu; in fullscreen the second Esc leaves fullscreen and the menu stays.
52. **The pause menu:** Continue (and P) resume; Restart restarts; change Volume, Music, Advanced info, Coaching tips and Camera view and see them apply; ⚙ More settings opens Settings and closing it comes back here; Level select and Main menu need two clicks. Fly into a stall with Auto-pause on: the menu shows the STALL explanation. On a phone the ❚❚ button (top corner, next to ⤢) opens it. Arrow keys do nothing to the plane while it is open.
53. **Quick settings everywhere:** change a setting in the pause menu, open Settings → Quick: it shows the same value; press `T` or `V` while paused: the boxes follow.
54. **The results screen:** on page 2, "🗺 Level select" opens that location's scenarios, "⌂ Main menu" the main menu, "Next" the next briefing.
55. **All screens in the three layouts** (desktop, `?layout=cockpit`, `?layout=portrait`) with Light, Dark and High contrast: main menu, level select, a location, How to play, pause menu. Tab stays inside each screen and every button is at least 44 px.

56. **Steering with the mouse:** on the main menu hold the mouse on the empty sky and move up: the nose rises, small force arrows appear, the hint fades (and stays gone after a reload). Clicking a button still just presses it.
57. **Steering by touch:** on a phone (or the device toolbar) drag up / down on the sky; the page does not scroll.
58. **Steering by keyboard:** click the sky, then ↑ ↓ pitch and ← → speed. Press Tab: focus goes to a button, the plane flies itself again, and the arrows now move between the buttons. Enter / Space only press buttons.
59. **Hand-back:** stop steering: after 5 s the plane levels out and cruises in slow waves again.
60. **A loop:** hold ↑ (or drag up and hold): the plane loops, the pilot grins upside down; it never leaves the screen or hits the ground.
61. **Locations:** with only the Grass strip open, the scene stays there. Turn on Teacher mode (Settings → Game) and wait 40–60 s: it cross-fades to the Coast (boats, lighthouse), then the Mountain and the Island.
62. **Night:** set your computer clock to the evening (or wait): dusk with a low sun, then night with stars, a moon and runway lights.
63. **Every plane on the menu:** pick each plane in the Hangar and go back: it flies in its paint with your pilot; the glider is silent, the fast jet quicker with its gear up.
64. **Reduce motion on:** the scene and the plane are still, there is no hint and the sky cannot be dragged.
65. **Dark and high contrast:** the scene follows the theme and the panel keeps the text readable.
66. **Portrait layout:** the plane cruises above the buttons, the ground sits at the bottom, the buttons stay clear.
67. **The animation stops during a flight:** start any flight; the menu scene stops (and starts again on the main menu).

68. **First visit:** clear the site data: after the main menu appears, "Hi, welcome to Flight School!" greets you; "Let’s go →" asks "How old are you?" with 6 to 10, 11 to 15 and 16 or older (each with an example sentence). Pick one, or "Rather not say" / Skip / Esc (Student); ← Back returns to the greeting. Reload: it does not come back, and no age is stored (only the level).
69. **1.1 at each level** (Quick settings → Explanations): Explorer: the coach says "Turn the engine up…", "Almost flying! Lift the nose up a little.", the panel shows "fast", "up high", "↑ going up" and "Lift is winning!", no numbers on the arrows; the results say e.g. "Pilot landed gently. Nice and soft!" with simple checks. Student: as before. Pilot: "Rotate: L/W = 0.88…", the pitch shows C_L, VERTICAL SPEED, and the results have "The numbers".
70. **A stall warning at each level:** raise the nose past the warning: Explorer "Too steep! Point the nose down a little!", Student "TOO STEEP!…", Pilot "STALL WARNING: angle of attack …". With Auto-pause on, the pause menu's STALL text follows the level.
71. **Switching mid-flight:** pause, change Explanations in the pause menu: the meters, labels and the next coach message change at once, the flight goes on.
72. **A lesson at Explorer and at Pilot:** Lesson 1 at Explorer uses the short words ("Weight (red arrow) pulls the plane down."); at Pilot the steps are as before and the finished card has "The physics". How to play → Lessons at Pilot lists the physics of every lesson.
73. **Metric units at Pilot:** Settings → Display → Units → Metric: km/h, m and m/s everywhere, also in coach messages and the results. The option is hidden at Explorer and Student, and they show kt / ft / fpm (Explorer none).
74. **An old save:** a browser with progress from before: stars, plane and pilot are kept, the level is Student, and the choice card appears once.
75. **Phones and big text:** `?layout=portrait` with Settings → Text size → Extra large at each level: coach messages, the panel words and the Pilot "The numbers" box wrap without overflowing ("The numbers" is closed by default on phones).

76. **Pause menu:** fly 1.1, press Esc: the small card with Continue focused. Restart restarts; 🔈 mutes (the icon and its label change) and the slider changes the volume; ⚙ opens Quick settings on top, ← Back or Esc returns to the pause card; ⌂ asks "Leave this flight?" (Stay / Main menu). Esc / P resume; in fullscreen (Chrome) the first Esc pauses, the second leaves fullscreen and the card stays. Fly into a stall with Auto-pause: one short STALL line on the card.
77. **Hangar on desktop:** both tabs fit without scrolling. Plane: click each plane in the row (the preview and bars change; the Glider on 1.1 shows 🔒 and why); pick a paint. Pilot: switch Skin / Hair / Face / Headgear / Jacket; the row under them changes; Random, Reset and the licence icon work.
78. **Hangar on phones:** the device toolbar at 812×375 (sideways) and 375×812 (upright): no vertical scrolling; the rows scroll with a swipe.
79. **Scrolling rows:** mouse wheel over a row scrolls it sideways; ‹ › buttons; focus an item and press ← →: focus moves and the row follows.
80. **Achievements:** the main menu shows 🏆 0/15 (your count); it opens the achievements; Back returns to the main menu. The level select no longer has it.
81. **Touch / keyboard:** in the device toolbar pick a phone and reload: no KEYS panel, How to play → Controls shows only touch, Settings → Controls has no key re-binding, coach says "Hold + (or tap FULL)…". Press a key on the real keyboard: the keyboard hints come back without the layout jumping.
82. **Rotating mid-flight:** in the device toolbar start a flight upright, then rotate: the layout changes to sideways and the flight carries on.

83. **One achievement:** with a fresh save, land 1.1 for the first time (First flight): the card slides down with a chime, then up after about 4 s.
84. **Two at once:** with a fresh save, make the first landing a soft one (under 100 fpm) to earn First flight and Butter together: the two cards come one after another. Hover one: it stays. Click it: the achievements list opens with it highlighted. × closes it early.
85. **Every panel opens and closes smoothly:** Settings (S), the pause menu (Esc) and its ⚙ card, the Hangar (G), How to play, level select, a location, the briefing, the results, the licence card, the achievements. Click open/close quickly several times: nothing gets stuck, and the last state wins.
86. **Reduce motion on:** the same panels just fade quickly; screens switch instantly; notifications fade without sliding.
87. **Centred screens:** How to play, the level select and a location sit in the middle of the screen; with Extra large text they scroll inside the box. Daily and Endless are centred under the location cards.
88. **Tags and the icon key:** on each location the cards show coloured tags (the Island has Night, Dusk, Carrier, Shear…; the plane tag only where another plane is suggested). Hover a tag; open ⓘ Icon key (Esc closes it).
89. **The briefing:** click a scenario: header with tags, Your goal steps, Conditions rows, You will learn, Plane with Change plane, Fly this scenario. No scrolling on desktop or at 740×360.
90. **Themes and layouts:** repeat 85, 88 and 89 with Dark and High contrast, at `?layout=cockpit` and `?layout=portrait`.

## Earlier versions

- **v11:** the landing runway is placed when you reach the target height (`placeRunway()`); missed approach result; landing on the grass after take-off ends the flight; a fifth quick-tour step on the landing lights.
- **v10:** a real landing runway with threshold, touchdown zone and overrun; glide-path lights (PAPI); five star checks; a debrief that quotes your flight.
- **v9:** keys card, quick tour, live checklist, force tips, 3-star results with replay and flight path, larger touch buttons.
