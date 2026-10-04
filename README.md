# Iron Rain

An armored-artillery game in the spirit of Scorched Earth, with a military look, in a single HTML file. No build step, no server.

**Play:** https://buckbiggles.github.io/iron-rain/

- 2–4 tanks, any mix of humans and CPU opponents, on a huge battlefield
- **5 maps** (the host picks in the armory, ▲/▼ or N): Rolling Hills, Mountain Pass, The Gorge, Steppe, Badlands
- Spawn points are random, except 1v1 and 2v2, which use fixed, tested positions
- WWII skies: fighters dogfight and bombers drone over in the background
- **Armory:** before the battle every player picks one of 8 tanks (Warhound, Bulwark, Jackal, Mammoth, Viper,
  Rhino, Scorpion, Kodiak — each with its own ARMOR, MOBILITY and ATTACK, the % of normal damage its shells deal)
  and a colour, then hits READY. CPUs pick at random.
- **Online multiplayer:** host a room, share the invite link or 5-letter code, friends join from their own browsers
- Local hot-seat play on one screen is still there too
- **Teams mode** (3–4 tanks): in the armory switch FREE-FOR-ALL → TEAMS and pick ALPHA or BRAVO; CPUs fill the smaller side.
  Last team standing wins and every member scores. Friendly fire hurts, but only hits on enemies earn a supply drop.
- Ground that behaves like loose sand: steep slopes slump, craters cave in, dirt piles spread into dunes
- **Underground caverns** on every map, home to little aliens: blasts nearby crack the roof (a few hits bring it down),
  then it caves in, the ground above sinks into the hole and any
  tank on top goes down with it, while the aliens escape in a flying saucer. Drills and orbital strikes collapse them at once
- No wind: shells fly on gravity alone. Four weapons: Missile, Big Bomb, Triple, and the **Drill** (2 per round), which bores straight
  through the earth to hit a tank behind a hill, burst out the far side, or break into a cavern and collapse it
- Land a hit, then type W, A, S, D in the random order shown, within 3 seconds, to spin the supply-drop wheel. Prizes go into your **stockpile** — keep as many as 8 and press **Q** (or click SUPPLY) to arm one when you want it:
  Nuke, MIRV, Dirt Bomb, Bouncer, **Lucky 7** (seven shells in a tight group), Teleport, Vampire, **Orbital Strike** (satellite laser),
  and four status shells that last through the victim's next turn: **Incendiary** (burning: 15 damage when it starts),
  **Cryo** (frozen: can't aim or drive), **Acid** (corroded: takes 50% more damage), **EMP** (shorted: half power)
- **Move after you shoot:** once your shot lands, drive with whatever fuel is left, or press ENTER to end your turn
- **After-action report** at the end of each round: damage, accuracy and kills for every unit

## Online play

1. Pick **HOST**, choose how many tanks (2–4), and send friends the invite link (or the room code).
2. Friends open the link, or pick **JOIN** and type the code.
3. Host presses **START**. Open seats are filled by CPU tanks.

The host's browser runs the game and streams it to everyone (WebRTC peer-to-peer through
[PeerJS](https://peerjs.com)'s free broker), so the host should keep their tab open.
If someone drops, their tank becomes a CPU.

## Controls

The control panel and a controls + ammo card sit in a strip below the battlefield, so nothing covers your tank. Click any ammo icon on the card to see what it does.

| Key | Action |
|---|---|
| ← → | Aim |
| ↑ ↓ | Power (hold Shift for fine) |
| A D | Drive (limited fuel) |
| 1 2 3 4 | Choose weapon |
| Q | Arm the next special from your supply stockpile (press again to cycle, past the last = none) |
| Space | Fire |
| Enter / E | After your shot: end your turn (or just drive until the fuel runs out) |
| W A S D | After a hit: press the 4 keys shown (W, A, S, D in a random order) within 3 s |
| T / M / P | Aim assist / sound / pause (offline only) |
| Armory | ←/→ tank, ↑/↓ colour, Enter ready, Tab next player (hot-seat) — or click |
| Esc | Menu / leave room |
