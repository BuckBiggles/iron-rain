# Iron Rain

An armored-artillery game in the spirit of Scorched Earth, with a military look, in a single HTML file. No build step, no server.

**Play:** https://buckbiggles.github.io/iron-rain/

- 2–4 tanks, any mix of humans and CPU opponents, on a huge battlefield
- **5 maps** (the host picks in the armory, ▲/▼ or N): Rolling Hills, Mountain Pass, The Gorge, Steppe, Badlands
- Spawn points are random, except 1v1 and 2v2, which use fixed, tested positions
- WWII skies: fighters dogfight and bombers drone over in the background
- **Armory:** before the battle every player picks one of 8 tanks (Warhound, Bulwark, Jackal, Mammoth, Viper,
  Rhino, Scorpion, Kodiak — each trading armor against mobility) and a colour, then hits READY. CPUs pick at random.
- **Online multiplayer:** host a room, share the invite link or 5-letter code, friends join from their own browsers
- Local hot-seat play on one screen is still there too
- **Teams mode** (3–4 tanks): in the armory switch FREE-FOR-ALL → TEAMS and pick ALPHA or BRAVO; CPUs fill the smaller side.
  Last team standing wins and every member scores. Friendly fire hurts, but only hits on enemies earn a supply drop.
- Ground that behaves like loose sand: steep slopes slump, craters cave in, dirt piles spread into dunes
- **Underground caverns** on every map: a blast nearby caves one in, the ground above sinks into the hole and any
  tank on top goes down with it (neighbouring caverns can chain-collapse)
- Wind, and four weapons: Missile, Big Bomb, Triple, and the **Drill** (2 per round), which bores straight
  through the earth to hit a tank behind a hill, burst out the far side, or break into a cavern and collapse it
- Land a hit, then type A-S-D-F within 3 seconds to spin the supply-drop wheel for a one-shot special:
  Nuke, MIRV, Dirt Bomb, Bouncer, Airstrike, Teleport, Vampire, **Orbital Strike** (satellite laser),
  and four status shells — **Incendiary, Cryo, EMP, Acid** — that leave the tanks they hit
  Burning / Frozen / Shorted / Corroded: **half power on their next shot**, then it wears off

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
| Space | Fire |
| A S D F | After a hit: press A, S, D, F in order within 3 s |
| T / M / P | Aim assist / sound / pause (offline only) |
| Armory | ←/→ tank, ↑/↓ colour, Enter ready, Tab next player (hot-seat) — or click |
| Esc | Menu / leave room |
