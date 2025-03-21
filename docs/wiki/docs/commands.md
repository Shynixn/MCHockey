# Commands

The following commands are available in MCHockey. You can access them by typing:

```
/mchockey help 1
```

### /mchockey create

```
/mchockey create <name> <displayName>
```

Creates a new arena for a MCHockey game.

* Name: Identifier of a game
* DisplayName: Arbitrary Display for your game. Can contain ChatColors.

### /mchockey delete

```
/mchockey delete <name>
```

Deletes a MCHockey game.

* Name: Identifier of a game

### /mchockey list

```
/mchockey list [player]
```

Lists all games you have created.

### /mchockey toggle

```
/mchockey toggle <name>
```

Enables or disables your game. If a game is disabled, nobody can join.

* Name: Identifier of a game

### /mchockey join

```
/mchockey join <name> [team] [player]
```

Lets the player executing the command join the game. If no team is specified, a random team will be selected.
If the player has already joined a game, this command can also be used to switch teams. 

* Name: Identifier of a game
* Team: Optional name of the team. Is ``red``, ``blue`` or ``referee``.
* Player: Optional name of the player to join. Requires the ``mchockey.edit`` permission to use.

### /mchockey leave

```
/mchockey leave [player]
```

Lets the player executing the command leave the game.

* Player: Optional name of the player to leave. Requires the ``mchockey.edit`` permission to use.

### /mchockey axe

```
/mchockey axe
```

Adds the MCHockey axe for selection to your inventory.

### /mchockey select

```
/mchockey select <name>
```

Sets a area for your arena.

* Name: Identifier of a game
* Type: Type of selection to set: e.g. field, blue_goal, red_goal. See tab completion for all values.

### /mchockey location

```
/mchockey location <name>
```

Sets a location for your arena.

* Name: Identifier of a game
* Type: Type of location to set: ball, red_spawnpoint, blue_spawnpoint, leave_spawnpoint


### /mchockey highlight

```
/mchockey highlight <name>
```

Starts highlighting your arena. When executing this command a second time, you stop highlighting an arena.

* Name: Identifier of a game

### /mchockey inventory

```
/mchockey inventory <name> <team>
```

Copies the inventory of the player executing the command. This copy will be applied to players when they join a game.

* Name: Identifier of a game
* Team: Name of the team. Is always red or blue.

### /mchockey armor

```
/mchockey armor <name> <team>
```

Copies the armor inventory of the player executing the command. This copy will be applied to players when they join a game.

* Name: Identifier of a game
* Team: Name of the team. Is always red or blue.

### /mchockey gamerule

```
/mchockey gamerule <key> <name> <value>
```

Sets a gamerule of MCHockey.

* Key: The name of the gamerule.
* Name: Identifier of a game
* Value: Value of a gamerule. See tab completions for all values.

### /mchockey sign

```
/mchockey sign <name> <type>
```

Enables the player to add a specific sign by right-clicking any sign. You can remove signs by simply breaking the block.

* Name: Identifier of a game
* Type: Type of sign to create. Possible values: join, leave, team_red, team_blue

### /mchockey referee startgame

```
/mchockey referee startgame
```

Starts the lobby countdown of a game.

### /mchockey referee stop

```
/mchockey referee stop
```

Transitions the game to the final period. Executing this command again stops it.

### /mchockey referee setball

```
/mchockey referee setball [x] [y] [z] [yaw] [pitch] [world]
```

Teleports the ball to the position of the referee.

### /mchockey referee setballrel

```
/mchockey referee setballrel [forward] [sideward]
```

Teleports the ball to the relative position of the referee.

### /mchockey referee whistleresume

```
/mchockey referee whistleresume
```

Resumes the game and sets the ball interactable.

### /mchockey referee whistlestop

```
/mchockey referee whistlestop
```

Stops the game and sets the ball inactive.

### /mchockey referee freezetime

```
/mchockey referee freezetime
```

Freezes the countdown and sets the ball inactive.

### /mchockey referee nextperiod

```
/mchockey referee nextperiod
```

Transitions to the next configured period.

### /mchockey placeholder

```
/mchockey placeholder <placeholder>
```

Tries to resolve the value of a given placeholder.

* PlaceHolder: PlaceHolder


### /mchockey reload

```
/mchockey reload [name]
```

Allows to reload all games or a specific single one.

* Name: Optional identifier of a game


