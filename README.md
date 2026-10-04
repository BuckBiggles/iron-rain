# Iron Rain

An armored-artillery game in the spirit of Scorched Earth, with a military look, in a single HTML file. No build step, no server.

**Play:** https://buckbiggles.github.io/scorched-tanks/

- 2–4 tanks, any mix of humans and CPU opponents, on a wide battlefield
- **Armory:** before the battle every player picks one of 8 tanks (Warhound, Bulwark, Jackal, Mammoth, Viper,
  Rhino, Scorpion, Kodiak — each trading armor against mobility) and a colour, then hits READY. CPUs pick at random.
- **Online multiplayer:** host a room, share the invite link or 5-letter code, friends join from their own browsers
- Local hot-seat play on one screen is still there too
- Ground that behaves like loose sand: steep slopes slump, craters cave in, dirt piles spread into dunes
- Wind, and three weapons (Missile, Big Bomb, Triple)
- Land a hit, then nail a 2-second W-A-S-D key combo to spin the supply-drop wheel for a one-shot special:
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
| 1 2 3 | Choose weapon |
| Space | Fire |
| W A S D | After a hit: press the 4 keys shown, in order, within 2 s |
| T / M / P | Aim assist / sound / pause (offline only) |
| Armory | ←/→ tank, ↑/↓ colour, Enter ready, Tab next player (hot-seat) — or click |
| Esc | Menu / leave room |
