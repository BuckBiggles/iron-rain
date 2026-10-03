# Scorched Tanks

A Scorched Earth-style artillery game that runs in a single HTML file. No build step, no server.

**Play:** https://buckbiggles.github.io/scorched-tanks/

- 2–4 tanks, any mix of humans and CPU opponents
- **Online multiplayer:** host a room, share the invite link or 5-letter code, friends join from their own browsers
- Local hot-seat play on one screen is still there too
- Destructible terrain, wind, and three weapons (Missile, Big Bomb, Triple)
- Land a hit and spin the prize wheel for a one-shot special attack:
  Nuke, MIRV, Dirt Bomb, Bouncer, Airstrike, Teleport, Vampire

## Online play

1. Pick **HOST**, choose how many tanks (2–4), and send friends the invite link (or the room code).
2. Friends open the link, or pick **JOIN** and type the code.
3. Host presses **START**. Open seats are filled by CPU tanks.

The host's browser runs the game and streams it to everyone (WebRTC peer-to-peer through
[PeerJS](https://peerjs.com)'s free broker), so the host should keep their tab open.
If someone drops, their tank becomes a CPU.

## Controls

| Key | Action |
|---|---|
| ← → | Aim |
| ↑ ↓ | Power (hold Shift for fine) |
| A D | Drive (limited fuel) |
| 1 2 3 | Choose weapon |
| Space | Fire |
| T / M / P | Aim assist / sound / pause (offline only) |
| Esc | Menu / leave room |
