# Creating a new game

This page explains step by step to setup a new game.

## Minimum required setup

### Create a new game

Execute the following command to create a new arena file.

```
/mchockey create game1 My first game
```

### Confirm that the arena has been created

Execute the following command to list all games:

```
/mchockey list
```

Output:

```
game1 [My first game] [disabled]
```

You can see that the arena is still disabled and cannot be joined yet.

### Get the selection axe

Get the mchockey selection axe for selecting playing areas and goals.

```
/mchockey axe
```

### Enable highlighting

You can toggle highlighting important areas when editing your game. This makes it easier to edit them.

```
/mchockey highlight game1
```

### Setting the playing field

Select ``Point A`` with left-clicking using the MCHockey axe and ``Point B`` with right-clicking using the MCHockey axe.
Then execute the command below.

![image info](./assets/arena7.png)


```
/mchockey select game1 field
```

### Setting the goal of team red

Select ``Point A`` with left-clicking using the MCHockey axe and ``Point B`` with right-clicking using the MCHockey axe.
Then execute the command below.

![image info](./assets/arena8.png)


```
/mchockey select game1 red_goal
```

### Setting the goal of team blue

Select ``Point A`` with left-clicking using the MCHockey axe and ``Point B`` with right-clicking using the MCHockey axe.
Then execute the command below.

![image info](./assets/arena8.png)


```
/mchockey select game1 blue_goal
```

### Setting the ball spawnpoint

Move to the location where you want the ball to spawn. The current location of your player is used as a value when you execute the ``/mchockey location``
sub command. Execute the command below.

```
/mchockey location game1 ball
```

### Enable the game

Once every location has been set, you can try to activate the game by executing the following:

```
/mchockey toggle game1
```

Confirm that the game is listed as enabled.

```
/mchockey list
```

Output:

```
game1 [My first game] [enabled]
```

You can join the game by running into the arena or executing the ``/mchockey join game1`` command.

## Optional steps

The following steps are not necessary but allow you to further customize the experience.

### Setting the leave-spawnpoint

Players can leave your game by running out of the field. However, you can also leave by typing ``/mchockey leave``, which causes the player
to be launched out of the forcefield. To avoid this, you should set a leaveSpawnpoint.

```
/mchockey location game1 leave_spawnpoint 
```

### Setting the team-spawnpoints

Currently, players spawn at the location of the ball. You should also set individual team spawnpoints.

Disable the arena to be able to move into it.

```
/mchockey toggle game1
```

Move to the first location and execute:

```
/mchockey location game1 red_spawnpoint
```

Move to the second location and execute:

```
/mchockey location game1 blue_spawnpoint
```

## Creating a Minigame

### Converting the HUBGAME to a MINIGAME

* Currently, players can join and leave a game at any time. The timespan of a game is also infinity. In order to convert it to a standard Minecraft minigame, with a lobby 
and a max time, you should execute the following command.
* If your arena has been enabled before, you may encounter and error message. You can ignore that because we will fix it in the next steps.

```
/mchockey gamerule gameType game1 minigame
```

### Setting the team-lobby-spawnpoints

Move to the lobby spawnpoints of your teams and execute the corresponding commands.

```
/mchockey location game1 red_lobby
```

```
/mchockey location game1 blue_lobby
```

### Enabling the game

If your game is disabled in the game list, you should now be able to enable it with the toggle command.

```
/mchockey list
```


```
/mchockey toggle game1
```

## Half-time, over-time 

You can configure periods like half-times, breaks and overtimes in your ``game1.yml`` file. See the further customization section below.

## Further Customizations

Further customization options can be found in the ``plugins/MCHockey/arena/<name>.yml`` file.

The ``arena_sample.yml`` file contains explanations for each property.

Execute the reload command to load your file changes.

```
/mchockey reload game1
```


