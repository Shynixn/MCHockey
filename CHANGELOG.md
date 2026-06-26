# Changelog

## Release 7.41.1

### Bugs/Issues

* #747 Fixed compatibility with Paper 26.2 builds.

---

## Release 7.41.0

### Changes

* Shynixn/BlockBall#527 Replacing the entire puck physics engine with the new 2026 puck engine. 
* Shynixn/BlockBall#527 All information can be found on this new [wiki page](https://shynixn.github.io/MCHockey/wiki/site/ball/)
* Shynixn/BlockBall#527 The puck is no longer tied to the arena and can be configured in the new ``plugins/MCHockey/ball`` folder.
* Shynixn/BlockBall#527 Added new puck properties and replaced existing ones to make it more realistic. 
* Shynixn/BlockBall#527 The puck can now be configured to have a realistic bounce, spin, and friction.
* Shynixn/BlockBall#527 The puck now bounces off walls and players in a more realistic way.
* Shynixn/BlockBall#527 The puck can be configured to allow grabbing and throwing. A sample puck called hand_puck.yml is included in the ``plugins/MCHockey/ball`` folder.
* Shynixn/BlockBall#527 Added configurable puck interactions. You can now configure to take sprinting, sneaking, selected hotbar slots, and more into account when interacting with the puck. e.g. the puck can be shot further while sprinting, the puck can do a left curve when the left slots are selected 
* Shynixn/BlockBall#527 The [developer api](https://shynixn.github.io/MCHockey/wiki/site/api/) has changed. You can now spawn pucks outside of games and use it for other minigames or purposes on your server.
* Shynixn/BlockBall#744 Added support for Minecraft 26.2
* Shynixn/BlockBall#743 Added a new flag to allow or deny block and items interactions during MCHockey in Minigame mode.

---

## Release 1.0.0

### Changes

* Initial release of MCHockey

---
