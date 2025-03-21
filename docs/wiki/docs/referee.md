# Referee

MCHockey offers a third game mode called ``refereegame``. This game mode is exclusive for **Patreon supporters**. (They are responsible for funding this feature :heart:).

This game mode is intended for server events where you have an admin or moderator control the flow of a MCHockey match by using the ``/mchockey referee ....`` subcommands.
Examples:

* The referee can resume/pause matches
* The referee can blow the whistle to block players interacting with the ball
* The referee can place the ball anywhere
* ...


## Setup

### Create a new game with gamerule minigame first

Go to the page [https://shynixn.github.io/MCHockey/wiki/site/game/](https://shynixn.github.io/MCHockey/wiki/site/game/) and perform all steps until you have got a game with gamerule ``minigame.``

### Setting the referee spawnpoint

Move to the location where you want the referee to spawn in the field.

```
/mchockey location game1 referee_spawnpoint
```

### Setting the referee lobby spawnpoint

Move to the location where you want the referee to spawn in the lobby.

```
/mchockey location game1 referee_lobby
```

### Converting the MINIGAME to a REFEREEGAME

In order to give the referee full control over the game, you need to convert the game type.

```
/mchockey gamerule gameType game1 refereegame
```

### Enabling the game

```
/mchockey toggle game1
```

## Gameplay

Players can join the game in the same way as before. However, the lobby countdown will not start until a referee has joined the game.

A referee can join the game using the following command:

```
/mchockey join game1 referee
```

### Starting the game

``/mchockey referee startgame``

### Controlling the game

The referee can control the game using the ``/mchockey referee...`` subcommands. You can take a look at the commands beforehand, but they
are also displayed hints for the referee during the game.

### Setting up whistle sounds and clickable items

Currently, there is no way to directly add a whistle sound or execute the referee commands via items using MCHockey.

However, you can still do that by following these steps:

* Install a third party plugin to bind commands to items (they are called ``Command Items plugins``, use google)
* Bind the referee commands ``/mchockey referee whistleresume`` and others to items
* Bind the ``/playsound`` vanilla minecraft command to these items to play a whistle sound
* Put the item in your inventory and execute the ``/mchockey inventory game1 referee`` command to put that item into the inventory, which is received by the referee on join.


