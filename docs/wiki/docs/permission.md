# Permission

The following permissions are available in MCHockey.

### Levels

* User: A permission all players can have.
* Admin/User: Depending on your server, you may give this permission to your players. If you are not sure, try to build
  your server around **not giving this permission** to your players.
* Admin: A permission only admins should have.

### Recommended Permissions

| Permission                           | Level | Description                                           |   
|--------------------------------------|-------|-------------------------------------------------------|
| mchockey.command                    | User  | Allows to use the /mchockey command.                 |   
| mchockey.join.*                     | User  | Allows to join all games.                             |
| mchockey.shyscoreboard.scoreboard.* | User  | Allows to see all mchockey scoreboards during games. |

### All Permissions

| Permission                                             | Level      | Description                                                                                          |   
|--------------------------------------------------------|------------|------------------------------------------------------------------------------------------------------|
| mchockey.command                                      | User       | Allows to use the /mchockey command.                                                                |   
| mchockey.join.*                                       | User       | Allows to join all games. The **mchockey.command** permission is also required.                     |  
| mchockey.join.[name]                                  | User       | Allows to join a specific game. The **mchockey.command** permission is also required.               |
| mchockey.command.staff                                | Admin/User | Allows to execute commands while ingame. This permission will be replaced in the future.             |  
| mchockey.game.inventory                               | Admin/User | Allows open and click in inventories while ingame.   This permission will be replaced in the future. |
| mchockey.edit                                         | Admin      | Allows to create, edit and delete games.                                                             |                          
| mchockey.referee.join                                 | Admin      | Allows to manipulate games using /mchockey referee commands                                         |  
| mchockey.shyscoreboard.scoreboard.*                   | User       | Allows to see all scoreboards                                                                        |
| mchockey.shyscoreboard.scoreboard.\[scoreboard-name\] | User       | Allows to see a specific scoreboard                                                                  |
| mchockey.shyscoreboard.command                        | Admin      | Allows to use the /mchockeyscoreboard command.                                                      |
| mchockey.shyscoreboard.reload                         | Admin      | Allows to reload configurations.                                                                     |
| mchockey.shyscoreboard.add                            | Admin      | Allows to add a scoreboard to a player                                                               |
| mchockey.shyscoreboard.remove                         | Admin      | Allows to remove a scoreboard from a player                                                          |
| mchockey.shyscoreboard.update                         | Admin      | Allows to refresh a scoreboard                                                                       |
| mchockey.mcplayerstats.command                        | Admin      | Allows to use the /mchockeystats command.                                                           |
| mchockey.mcplayerstats.reload                         | Admin      | Allows to reload configurations.                                                                     |
| mchockey.mcplayerstats.login                          | Admin      | Allows to start a login session                                                                      |
| mchockey.mcplayerstats.collect                        | Admin      | Allows to collect stats manually                                                                     |
| mchockey.mcplayerstats.upload                         | Admin      | Allows to upload data manually                                                                       |
| mchockey.mcplayerstats.cleanup                        | Admin      | Allows to cleanup data manually                                                                      |
| mchockey.mcplayerstats.schedules                      | Admin      | Allows to display schedules                                                                          |
| mchockey.mcplayerstats.preview                        | Admin      | Allows to preview pages                                                                              |



