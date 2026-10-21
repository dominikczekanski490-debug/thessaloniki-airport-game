# Fraport Greece SKG – v7 overnight progress

## v7.1 – Heathrow-scale airport (LIVE)
- Six new terminals T1–T6 next to the original Makedonia terminal (kept as-is).
  - T1 Aegean/Star Alliance, T2 low cost (Ryanair/Wizz/easyJet/Volotea), T3 Jet2/TUI/charter, T4 Middle East & long haul, T5 Fraport flagship hub (3 piers), T6 satellite between the runways (train only).
  - 572 new check-in desks on 26 islands with airline zone signs and dense instanced queues.
  - Security lanes, airside plazas with ~100 brand storefronts (Hellenic Duty Free, Mikel, Coffee Island, Everest, Starbucks, McDonald's, Burger King, Zara, Victoria's Secret, Swarovski, Apple, LEGO, Hamleys, Pandora, Boots, WHSmith, Public, Greek deli, souvenirs…). Shops are enterable, with counters and goods; Ⓐ to buy.
  - Fun facilities: arcade, cinema, kids' play, spa & pool, gym, aviation museum, indoor garden + waterfall, VR flight sim, pod hotel, bowling, observation deck.
  - Keycard staff doors (they open in v7.4).
  - 172 new gates (A–F) on piers with moving walkways, jet bridges and instanced parked planes in airline colours.
- Second parallel runway (z −560), new taxiways, extended runway 1, apron for all terminals.
- Driverless terminal train on a viaduct with 7 stations (rideable, Ⓐ at 🚆), plus 🗺️ fast travel and an airport-wide map.
- Hundreds of walking people, plus thousands of instanced queuing and seated passengers.
- Performance: the static Makedonia scene is merged per 100 m chunk by material (about 1650 meshes become about 230). Planes and vehicles are compacted. Terminals are streamed by distance. Draw calls: 40–140 at ground level, about 140 in a full aerial view.
- Best screenshot: shots/v7-aerial.png (also v7-t1ck.png, v7-aerial2.png)

## v7.2 – Thessaloniki city & EO16 highway (LIVE)
- EO16 airport road: six lanes with a central barrier, lamps, and green Greek motorway gantry signs, Greek over English. Signs: Θεσσαλονίκη / Thessaloniki, Κέντρο / Centre, Αεροδρόμιο ✈ Airport, Περαία, Ν. Μουδανιά, junction numbers 1–6, distances, and a welcome sign.
- Traffic: 90 instanced cars and three blue OASTH 01X buses on a loop airport ⇄ city.
- Drivable cars: your car, a rental car and taxis. Walk up to one and press Ⓐ: 0–130 km/h, camera chase.
- Stylised Thessaloniki:
  - About 110 city blocks of polykatoikia apartment buildings with balcony and window facades, shopfront awnings, rooftop tanks and street trees.
  - Aristotelous Square with its arcaded neoclassical buildings, the Nea Paralia promenade with trees, lamps and the Umbrellas sculpture, the White Tower, and the sea.
  - The port with cranes, containers and a ferry; hotels (Makedonia Palace, Electra Palace, Hyatt Regency) and Mediterranean Cosmos.
  - Metro stations (Ⓜ️ fast travel incl. an airport extension), plus people on the square and the promenade.
- Bus 01X stops at Makedonia, T1, T5 and Aristotelous. Ⓐ to ride; it fades and teleports, and riders count as airport passengers.
- The city grows with the airport: districts unlock as total passengers and upgrades rise.
- Fast travel now includes city spots. City draw calls: about 20–35 (merged per growth ring).
- Best screenshots: shots/v7-hwy.png (gantry signs + traffic), shots/v7-aerialcity.png, shots/v7-aris.png

## v7.3 — Fly the planes (live)
- Fly from any gate (plane icon), parked Makedonia planes, a runway, or a 7 km final (Fast Travel → ✈️ Fly a plane)
- Pushback, taxi, takeoff; arcade physics: joystick, throttle slider, FLAPS, GEAR, optional GYRO
- Chase, cockpit and tower cameras; HUD showing speed, altitude, heading, vertical speed, attitude ball, ILS glide path diamonds
- Scenery: Thessaloniki, Thermaic Gulf, Olympus, Pieria, Halkidiki, clouds
- Land on either runway for a score (sink rate, centreline) with cash and XP; gentle crash fades back to the approach
- ROUTE flights to ATH/HER/MAN/JMK teleport you to the destination final; ATC voice lines (speechSynthesis)
- Perf: screen-size culling while flying (about 420 draw calls on final; about 700–880 low over the airport)
- Best shots: shots/v7-fly-approach.png, v7-fly-olympus.png, v7-fly-cockpit.png, v7-fly-score.png

## v7.4: 25 major features (live)
- 🎮 FUN button and a "What's new in v7" screen listing all 25 features (it opens automatically once)
- Staff keycard (€5,000) opens every 🔒 staff door in every terminal and leads to the new Ops & Staff Zone east of the runways. It has 8 rooms:
  - Baggage hall: animated conveyors and a sorting game
  - Security CCTV: a spot-the-threat game
  - Canteen: an energy meal
  - Crew briefing: pick a route and fly it
  - AOC dashboard: weather, drills, VIPs and crowd events
  - Police: a case game
  - Cleaning depot: spill-cleaning shifts
  - Service tunnel: links to T6 and the hangar
- Maintenance hangar with a plane under service and a checklist game
- Fire station with a drivable 🚒 fire truck; apron fire emergencies (drive close to put them out)
- 3D weather: rain, snow, fog and storms with lightning. De-icing pad game
- Control tower ATC sequencing game. Flyable 🚁 helicopter (UP/DOWN buttons) and heliport
- VIP/private jet FBO with charters. Cargo hub with a cargo tractor and a freighter-loading game
- Construction mode with 8 props, saved
- Photo mode with filters and PNG save
- VIP motorcades to escort. Crowd events (PAOK/Aris fans, festivals)
- Airport Express rail between the airport and Thessaloniki Central
- Alliance deals (passive income)
- Seasonal decorations (Christmas, Oxi Day, summer and more)
- Playable facilities: arcade, bowling, cinema, museum quiz, VR flight
- 20 achievements, local leaderboards, and a 9-chapter story campaign
- Perf: plane parts baked into one vertex-colour mesh (14 → about 5 draw calls per plane). Flight over the airport: about 1,070 → about 530 draw calls
- Best shots: shots/v7-whatsnew.png, v7-bhs.png, v7-heli.png, v7-crowd.png, v7-firetruck.png

## v7.5: Mission board, live events, polish (live)
- 📋 Mission board at Makedonia and in every terminal: 3 active missions from a pool of 18, progress bars, swap, cash and XP rewards (also in FUN → Missions)
- ⏱️ A live event every minute (skipped while flying or when a menu is open): apron fires, bird strikes, VIP motorcades, fan crowds, weather changes, flash sales (triple payout), lost children, golden suitcases (€5,000), celebrities, record days, parking bonuses, extra Airport Express trains. Each has a 📍 Go button
- What's new now lists 27 items and reopens once for v7.5. Event banner sits below menus. Quick games stop when their menu closes
- Perf: final approach 298 draw calls, after landing on the runway 359, low over the airport about 500. Walk mode 100–145 at Makedonia
- Best shots: shots/v7-missions.png, v7-event.png, v7-whatsnew2.png

## v7.6: Better signs & graphics (live)
- New sign atlas: navy #0e1a3a, rounded corners, thin border, yellow-green Greek over bold italic English, round yellow vector pictograms (plane, passport, security, baggage, toilets, exit, train, taxi, food, info), yellow arrows, emissive backlight, high-res with max anisotropy
- Wayfinding signs hang from ceiling rods in framed boxes with depth and a back face
- Gate signs: navy boxes with teal/lime/yellow number circles and "Πύλη / Gate"
- Green exit signs. More junction signs in all 6 terminals (hall, plaza, piers, satellite)
- Highway: hi-res green Greek motorway signs (white Greek over italic English), route shields E90/A25/16/E75, junction boxes, arrows and km
- Graphics:
  - New sky with sun glow and clouds, plus a sunset sky (17:00–19:30, 05:30–07:30) with warm sun and ambient light
  - Exposure lowered, so less washed out
  - Sky environment reflections on floors and glass
  - Warm ceiling light strips, facade fins and transoms, roof skylights and fascia, forecourt canopies, planters
- Perf: merge pass now merges by material properties (not just identity): 1,653 meshes merged into 234. Walk mode 57–102 draw calls
- Shots: shots/v76-pier.png, v76-gates.png, v76-plaza.png, v76-sunset.png, v76-hwy.png

## v7.7: Graphics, boards, gate screens, planes, traffic, density, staff areas, duty free (live)
- Graphics: daytime light rebalanced (lower ambient, stronger sun, more contrast and shadows), colour grade (saturate 1.18, contrast 1.08), material tweaks
- Editable flight boards: departures and arrivals boards in every new terminal hall, plaza, pier and T6. Walk up and tap to edit flight number, airline, Greek/English destination, time, gate and status. Saved, and every board and gate screen in that terminal updates. The live schedule rolls on automatically
- Gate screens at all 172 new gates: airline colour bar and name, gate circle, flight, time, destination GR/EN, live status. Editable
- New plane model: lathe fuselage, nose and cockpit windows, window line, swept wings with dihedral, winglets, flap-track fairings, nacelles with fan face, spinner and exhaust, swept tailplane, airline-coloured fin, cheatline and engines. Strobes and nav lights
- Traffic: 16 more instanced planes landing and taking off on both runways, with wingtip and strobe lights (3 draw calls)
- Density: about 260 queueing people, about 470 seated at gates, staff in uniform, and more walkers per terminal. Kiosks, vending, charging, ad screens, art, info desks, planters
- Staff areas: a back-of-house interior next to every terminal (T1–T6), reached through the keycard door, no teleport. Corridor, baggage make-up with conveyors and carts, staff room, security office, stores; "ΜΟΝΟ ΠΡΟΣΩΠΙΚΟ / STAFF ONLY" signs
- Duty free in Makedonia and every terminal styled like the photo: cream floor, curving grey walkway, black ducted ceiling, white floating islands with spotlights, blue LED strip, hundreds of red paper birds, TOM FORD gondolas, BOSS lemon towers, brand-bay wall (ARMANI, LANCÔME, CHANEL, DIOR, ESTÉE LAUDER) with screens, GREEK PRODUCTS
- Shots: v77-dutyfree*.png, v77-gatescreen.png, v77-board-editor.png, v77-flight-edit.png, v77-busy.png, v77-staff.png, v77-planes.png, v77-plane-flying.png

## v7.8
- Staff-only doors (yellow/red STAFF ONLY · ΜΟΝΟ ΠΡΟΣΩΠΙΚΟ) in every terminal + Makedonia; free keycards at info desks; minimap locks, hint, FUN-hub staff button; walk-through tested.
- Makedonia staff building: control tower ops, crew room, canteen, 42 m tower; ramp door to airside service road.
- 7 new airlines/liveries, Makedonia boards in editor, per-type planes (A320/A321/737/A330/777), gear retracts, wide-body traffic.
- Fraport Greece branding, car parks, service road, GSE, remote stands R1–R12, cargo freighters; city: promenade, Rotunda, Arch, domes, boats/ferry.

## v7.8.1
- iPhone fix: 3D dropped back to 2D because canvas/texture memory (~500MB+, 4096x8192 sign atlas) blew past iOS Safari limits. Mobile now draws big canvases at half res (max 1024), pixel ratio cap 1.5, 1024 shadow map; webglcontextlost/restored handled (pause + restore instead of dying).

## v7.9
- Fix: landing/flyable plane showed a second fuselage+tail beside it (old textured livery parts shifted 1.9 m) - removed.
- Big dep/arr boards at entrances, check-in and security in T1-T5, larger ones in T6; 2D 📋 button shows boards for all terminals.
- Forecourt road network: lane markings, median, curbs, zebras, gantries, coach bays, island shelters, lamps; service road markings; west flyover interchange.
- Lane traffic with car-following and smooth turns (forecourt + city loop), better car model, no overlaps.
- Hotel coaches (8 hotels) with boarding passengers; ride to the city.
- Staff rooms: lockers, bench, kitchen, dining tables, sofa lounge + TV, notice board, rota.
- Halls: mezzanine cafes on both sides with escalators, atrium trees and lights, LED wall. Mobile: fewer cars/coaches/passengers.

## v8.0
- Photo-style signs on every terminal + Makedonia, landside and airside: dark angled canopy, purple-blue lit soffit, glowing THESSALONIKI + AIRPORT MAKEDONIA / TERMINAL n, 6-blade star logo; brighter at night.
- Continuous day/night from the game clock: sun path, sky/fog colour, golden sunrise/sunset, moon, lights at dusk; 🕒 time panel (sunrise/noon/sunset/night, 1-60x).
- Wayfinding: road gantries (Terminals, Makedonia, T6 train, parking, rent a car, cargo, hotels, city, exit), pedestrian blades.
- Walkable mezzanine cafe decks with escalator ramps in T1-T5.
- Drivable cars at every terminal forecourt (A to enter/exit, joystick/keys), road link to the city via the highway.

## v8.1
- 11 drivable apron jobs with beacons/HUD (fuel, catering, bags, follow-me, remote bus, turnaround, cargo K-loader, bird sweep, fire, ambulance, diversions); depots at T1 apron, remote stands, fire station.
- Stations: X-ray, passport, baggage routing, lounges, hotel (new hotel tower), K9, tower clearances, snow ops, passenger chats, PA announcements, cleaning robots, lost luggage hunt, air show.
- Finances charts, reviews/rating, career ranks, first-person view, K9 pet follower; 16 new missions; 🧰 hub.
- Fixes: no sun jump at sunset/sunrise, window glow fades gradually at dusk.
- PA rooms: 2 enterable announcement rooms in every terminal (T1-T6) and Makedonia; desk, mic, console, signage; 6 Greek+English presets (boarding, final call, gate change updates boards, delay, lost child, security) with chime, voice in that terminal and subtitles.

## v8.2
2D parity: T1–T6 walkable 2D areas (forecourt w/ THESSALONIKI star sign, check-in w/ live boards, mezzanine café, security/passport, airside plaza, Hellenic Duty Free, food court, gate piers with gate screens), staff-only doors + keycard, staff room / baggage make-up / security office, 2 PA rooms per terminal + Makedonia, staff building (crew room, tower), airport road + hotel, top-down driving (roads + apron jobs sharing JOBS12), 2D lost-luggage hunt, day/night tint + lights, map teleport. E-ink: no tint, 8fps driving.

## v8.3
PA sound chain (band-pass, saturation, compressor, generated hall IR, 4 delayed speaker echoes, ding-dong chime, muffled in staff rooms/outside), hold-to-talk mic (MediaRecorder + webkitSpeechRecognition en-GB), EN→GR templates + MyMemory fallback, el-GR TTS, typed fallback; 2D airline check-in desks; img/ + favicon 404 fix.

## v8.4
Jump button (Space) in 2D hop + 3D gravity arc; PA teleport button + map/TRAVEL entries, auto keycard.

## v8.5
iOS Greek TTS fix (gesture unlock, queued EN+GR, el voice prefix, install hint, test button), PA flight board + scripts, SKG Airport phone app (public + staff tabs), charging kiosks, keycard by default, 2D-only empty departures fix.

## v8.6
Greek translates actual transcript (fuzzy script match ≥ threshold, protected tokens, city map), Greek via meSpeak (lazy mespeak-el.js, ~1MB gz) through PA chain with toggle, monorail 3D+2D, distinct terminal identities (roofs/cladding/2D backdrops/shops), SKG app 2.0 (home, favourites+notifications, live map, boarding pass, weather, security waits, ops KPIs, delays chart, roster).

## v8.7
- Level-2 Grand Hall annex per T1–T5 (T1–T4 27,840→66,990 m² 2.41x; T5 41,760→98,310 m² 2.35x), kerb ramp, monorail platform; T6 satellite kept.
- T7 construction site (cranes, frame, hoardings, workers, diggers/trucks), build progress, monorail station, 2D/3D/maps/app.
- Walk-in shops (shelves, products, tills, staff) 2D+3D.
- Planes: curved taxi, pushback, rotation/climb, banked approach, flare. Cars: rounded loops, crossing stops, kerb stops, vehicle types, smoother player handling.
- SKG app: status pills, tails, flight detail progress/timeline/gate route, live map planes, banners, dark mode, pull-to-refresh.
- Estimated / Εκτιμώμενη column on 3D boards, gate screens, 2D boards, PA board, SKG app; delay field in board editor + staff delay.

## v8.8 (Part A)
- Greek PA reliability: built-in Greek voice (meSpeak buffer → Web Audio PA chain) by default, Melina optional; robust iOS speech queue (chunks, kept refs, cancel/resume, onstart retry, watchdog); audio session handling after mic; Greek always available (MyMemory → Google → template → generic); stricter script match (≥85%); on-screen PA log.
- T1A domestic/Balkans terminal (6 gates D1–D6, own boards/gate screens/app), 2D + 3D.
- T7 finished: 12 gates, planes at all gates, Fraport look (dark canopy/purple soffit, star logo, letters, yellow wayfinding), crowds/queues, shops; grand opening event; monorail "Terminal 7".
- City rebuild overlay: balconies, shopfronts/awnings, neoclassical fronts on Egnatia, lane markings, lamps, signs, ferries, moving cranes, instanced traffic with lights, sidewalk crowds; full city shown.
- Fixes: What's new popup, duplicate banner, airline check-in desks in 2D, board layout, livery details, smoothed flight controls.

## v8.9 – Part B: 15 gameplay features (LIVE)
- 🎮 Ops centre hub (HUD button, or the door from T1 check-in in 2D): career, ATC, events/strikes/storms, build mode, airline negotiations, night shift, hangar, customs, VIP, lost passengers, weather radar, passenger flow, museum and deck, story mode, spotting book (📷).
- The hangar, museum and customs interiors are built when you enter and freed when you leave. Mobile texture memory: 143MB.
- T7/T1A teleport buttons in travel and the map; PA rooms: T7 ×4, T1A ×1 (picker and nearest-room logic, in 2D and 3D).
- Signs never show mirrored text (unmirrored back faces). Gate screens and flight boards can be read from both sides (seating and walkway).
- T7 gate lounges filled: 6 seat rows, carpet, gate desk, screens, seated and standing passengers.

## v9.0 Part A – Greek PA says exactly what you said + bigger T7 (LIVE)
- PA: your actual transcript gets a fresh translation each time (Google, then MyMemory). There is no script or template substitution unless nothing was transcribed, and no cached or reused Greek. Older announcements are cancelled by a session id. The log shows transcript and translation.
- Voice: natural neural Greek audio (Google TTS), split into sentences with pauses, plus delayed "terminal speaker" echoes and hall ambience. Fallbacks: the best iPhone Greek voice (Premium/Enhanced Melina first), then the built-in offline voice. Lighter muffling.
- T7: 500 m wide, 16 gates, 16 shops/restaurants/lounge, food court and lounge & art garden (2D areas t7f, t7l), olive-tree planters, sculptures and art walls, sofas, 4 extra double-sided board pairs, more passengers.
- Teleports: Terminal 7 and T7 PA1–PA4 (plus T1A PA) in the PA picker, travel menu and 2D map, in both modes. Keycard from the first frame.

## v9.0 Part A2 – new SKG/Fraport UI (LIVE)
- Navy, white and gold glass UI in 2D and 3D. A bottom dock groups everything into 5 categories (Κίνηση/Move, Ανακοιν./PA, Επιχειρ./Ops, Εφαρμογή/App, Χάρτης/Map). Each one opens a flyout of large buttons (60px or more). RUN, JUMP and Action stay in the right-hand cluster.
- Top status bar (Greek above English): terminal or area, time, day, weather. In 3D, a mini-map with a compass rotates with the camera (T7 in gold).
- Smooth modal and flyout transitions. E-ink: high-contrast black and white, no blur, no animation, no mini-map.

## v9.0 Part B1 – scope on every announcement, synced broadcast, drills & evacuations (LIVE)
- Every announcement, whether live, typed, script or alarm, asks "📡 All terminals" or "📍 Only this terminal". There is no default, and Cancel stops it. "All" plays one shared audio buffer on one clock for all 9 terminals, and the PA log records the synced start, the end, the terminal list and the duration.
- Drills and REAL evacuations: from Ops (🚨 in the Ops flyout), the Ops centre, and the PA room. The scope is asked each time, including for the all-clear. Effects:
  - Siren, red screen pulse, flashing red beacons, green ΕΞΟΔΟΣ/EMERGENCY EXIT signs and floor arrows (3D).
  - Crowds walk out to the landside assembly points, with an evacuated % and a timer.
  - Alarm PA in Greek first, then English.
  - All clear restores everything. Drills are scored.
  - 2D: an exit arrow banner, a "Guide passengers" action and the same panel.
- UI: the old info card and task pill are folded into the status bar. 👤 moved to the App flyout, flyout buttons have Greek and English labels, weather is shown in Greek and English, the old mini-map is hidden in 3D, and PA subtitles show Greek above English.

## v9.0 Part B2 – bigger terminals, hotel interiors, SKG app tabs (LIVE)
- Every terminal is bigger: walkable Level 2 lounges (Σαλόνι, food hall, kids zone, books) above the airside plaza in T1–T5 and T1A. In 3D you reach them by escalator ramps or the ⬆️ item; they have seating, crowds and plants. In 2D: areas t1l2–t5l2 and t8l2, with ⬆️ doors from the airside areas. T7 was expanded in Part A.
- Makedonia Palace hotel interior (3D, built on entry and freed on exit; enter at the hotel tower door): lobby and reception, sofas, 3 lifts (floors G–8), a corridor with 12 rooms per floor (bed, TV, window, doors), restaurant and bar. 2D: hot27, hot27c, hot27r. Booking, resting and dining all work.
- SKG app tabs: 🚨 Alerts (live evacuation status, start a drill, latest PA in GR/EN), 🏨 Hotel (book, go to the hotel), 🗺️ Terminal maps (per-terminal zones + go), 📡 PA control (type an announcement, then All/Only this terminal; drill; PA rooms; log).
- Evacuation: crowds follow waypoints to the nearest doors. Landside goes out through the front doors to the forecourt; airside goes out to the apron between the piers. 2D shows small figures walking to the exit. The objective pill is folded into the status bar, and the dock hides while a modal or the app is open.

## v9.0 Part B3 – the 8 extras (LIVE)
1. Baggage reclaim hall (3D, built on entry and freed on exit; 2D area bag28): 3 working belts with moving bags, flight screens, crowds; find-the-bag and lost-luggage desk claims.
2. Staffable security checkpoint (3D; 2D sec28): 4 lanes with x-ray tunnels, arches, moving trays and queues that grow and shrink. Open/close lanes, x-ray screen, bag-search mini-game, live wait times in a HUD.
3. Fire station by T1 with 3 trucks. They drive to the runway on any drill or evacuation, storm event or manual dispatch, with flashing lights, and return on all clear (2D fire28 with animated trucks).
4. Bus station with OASTH 01X/01N buses (they arrive and leave) and a taxi rank with Thessaloniki blue-and-white taxis you dispatch (2D bus28); ride the bus to the city.
5. Gate boarding sequence at any gate: Greek and English boarding PA (asks the scope), a queue, scanned passes, a jet bridge, doors close, pushback (3D); same flow in 2D gate areas.
6. Seasonal events: Christmas trees, lights and banner; Easter red eggs and candles; summer peak with umbrellas, +40% crowds and income. Auto by date or chosen in Ops → 🎄 Seasons (2D overlay banners).
7. SKG FM 98.1 airport radio (PA flyout 📻) with generative music and flight/weather bulletins; music in shops in both modes, fading with distance.
8. 🏆 Trophies tab in the SKG app (13 new achievements, bronze/silver/gold tiers, progress) plus a trophy cabinet in T7.
- Hotel polish: wood-floor lobby, patterned red-gold carpet, warm walls and wainscot, chandeliers, a showcase room (headboard, duvet, pillows, lamps, window, art, rug). The status bar shows "Ξενοδοχείο Makedonia Palace / Makedonia Palace hotel".
- Evacuation is faster and time-based (one-terminal REAL reaches about 87% at 60 s even at 5 fps in headless tests).

## v9.0.1 – quick fixes (LIVE)
- An always-visible 3D/2D toggle button at the top right in both modes (large touch target, e-ink variant).
- His own announcements no longer show any on-screen subtitle or caption, and the live transcript in the PA room shows only "Recording…". The text stays in the PA log only.

## v9.0.2 – iPhone PA audio + no covered buttons (LIVE)
- Audio is unlocked inside the All/Only-this-terminal tap itself (AudioContext resume + silent buffer, silent speech warm-up, silent <audio> play) and no longer cancels the new utterance.
- English always plays first: his recording, then iPhone en-GB speech, then the offline voice. Greek follows: Google neural TTS, then iPhone Melina, then the offline voice. Every step has a timeout, and the step list goes into the PA log.
- The A, Run and Jump buttons plus a new 📢 PA quick button sit on top (z 72) in a reserved row above the dock in portrait. In landscape the dock moves left and the buttons sit bottom-right. Flyouts open above them. Checked at 393x852 and 852x393 in 2D and 3D.
