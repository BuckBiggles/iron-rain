# Iron Rain

An armored-artillery game in the spirit of Scorched Earth, with a military look, in a single HTML file. No build step, no server.

**Play:** https://buckbiggles.github.io/iron-rain/

- **Campaign:** eight single-player missions, from a lone scout to an Expert final battle, each with its own map,
  weather, enemy (and sometimes allied) tanks and air support. Earn up to 3 stars per mission; progress saves in your browser
- 2–4 tanks, any mix of humans and CPU opponents, on a huge battlefield
- **CPU difficulty** (picked in the armory, ◀ ▶ or C): Easy, Normal, Hard or Expert — sharper aim, surer auth codes,
  and smarter use of drills and supply specials as it goes up
- **5 maps** (the host picks in the armory, ▲/▼ or N): Rolling Hills, Mountain Pass, The Gorge, Steppe, Badlands
- Spawn points are random, except 1v1 and 2v2, which use fixed, tested positions
- WWII skies: fighters dogfight and bombers drone over in the background
- **Armory:** before the battle every player picks one of 8 tanks (Warhound, Bulwark, Jackal, Mammoth, Viper,
  Rhino, Scorpion, Kodiak — each with its own ARMOR, MOBILITY and ATTACK, the damage a direct hit with the basic Missile does: 41 for the Bulwark up to 50 for the Viper; other shells scale the same way)
  and a colour, then hits READY. CPUs pick at random.
- **Online multiplayer:** host a room, share the invite link or 5-letter code, friends join from their own browsers
- **Store:** earn money in battle ($20 per hit, $30 per kill, $100 per win) and spend it on cosmetics: camo patterns
  (17, from Woodland to Galaxy), emblems, antenna flags, shell trails (11, from Frostbite to Stardust) and death effects
  (Party Popper, Ghost, Fireworks, Black Hole, Mushroom Cloud). Looks only; your money and upgrades are saved in this browser
- **Name your tank:** click your unit's name in the armory and type (up to 12 characters); your name is remembered
- **Opening supply drop:** every tank gets one free spin of the supply-drop wheel at the start of its first turn
- Local hot-seat play on one screen is still there too
- **2v2 Teams** in one click: pick **2v2** next to the tank counts (Local or Host), or in any 3–4 tank game switch
  FREE-FOR-ALL → TEAMS in the armory and pick ALPHA or BRAVO; CPUs fill the smaller side.
  Last team standing wins and every member scores. Friendly fire hurts, but only hits on enemies earn a supply drop.
- Ground that behaves like loose sand: steep slopes slump, craters cave in, dirt piles spread into dunes
- **Underground caverns** on every map, home to little aliens: blasts nearby crack the roof (a few hits bring it down),
  then it caves in, the ground above sinks into the hole and any
  tank on top goes down with it, while the aliens escape in a flying saucer. Drills and orbital strikes collapse them at once
- No wind: shells fly on gravity alone. Four weapons: Missile, Big Bomb, Triple, and the **Drill** (2 per round), which bores straight
  through the earth to hit a tank behind a hill, burst out the far side, or break into a cavern and collapse it
- Land a hit, then key in the four arrows shown (in a random order) with the arrow keys or W A S D: you get 1.5 seconds, plus a quarter second for every right key, to spin the supply-drop wheel. Prizes go into your **stockpile** — keep as many as 8 and press **Q** (or click SUPPLY) to arm one when you want it:
  Mini Nuke, MIRV, **Dig Bomb** (blasts a massive pit, tanks fall in), Bouncer, **Lucky 7** (seven shells in a tight group), Teleport, Vampire, **Orbital Strike** (satellite laser),
  and four status shells that last through the victim's next turn: **Incendiary** (burning: 15 damage when it starts),
  **Cryo** (frozen: can't aim or drive), **Acid** (corroded: takes 50% more damage), **EMP** (shorted: half power)
- **Move after you shoot:** once your shot lands, drive with whatever fuel is left, or press ENTER to end your turn. You can also set your angle and power for your next shot while you drive
- **Music:** a procedural military march, fuller on the menus and softer in battle; Esc menu toggles music and sound effects separately
- **Secret aim:** on an opponent's turn their angle and power read ??
- **After-action report** at the end of each round: damage, accuracy and kills for every unit

## Online play

1. Pick **HOST**, choose how many tanks (2–4), and send friends the invite link (or the room code).
2. Friends open the link, or pick **JOIN** and type the code.
3. Host presses **START**. Open seats are filled by CPU tanks.

The host's browser runs the game and streams it to everyone (WebRTC peer-to-peer through
[PeerJS](https://peerjs.com)'s free broker), so the host should keep their tab open.
If a friend drops out, a CPU minds their seat and their game keeps trying to reconnect for 45 seconds.
They can also rejoin any time with the same code or invite link (or just refresh the page): they get their
own seat back, in the lobby, in the armory (with their tank and colour) or mid-battle. A newcomer can take over
a dropped player's seat once the game has started.

## Controls

The control panel and a controls + ammo card sit in a strip below the battlefield, so nothing covers your tank. Click any ammo icon on the card to see what it does.

| Key | Action |
|---|---|
| ← → | Aim (90° is straight up; the barrel sweeps the 180° above its hull, so on a 30° slope that is 30–210° and you can aim below level) |
| ↑ ↓ | Power (hold Shift for fine) |
| A D | Drive (limited fuel) |
| 1 2 3 4 | Choose weapon |
| Q | Arm the next special from your supply stockpile (press again to cycle, past the last = none) |
| Space | Fire |
| Enter / E | After your shot: end your turn (or just drive until the fuel runs out) |
| ↑ ← ↓ → or W A S D | After a hit: enter the 4 arrows shown, in order: 1.5 s, +0.25 s per right key |
| M / P | Mute all (music + sound effects) / pause (offline only) |
| Armory | ←/→ tank, ↑/↓ colour, Enter ready, Tab next player (hot-seat), N map, C CPU difficulty, G mode — or click |
| Esc | In a game, the armory or an online lobby: menu with resume, settings (music, sound effects, volume, screen shake, film grain) and leave |
