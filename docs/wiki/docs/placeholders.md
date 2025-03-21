# PlaceHolders

The following placeholders are available in MCHockey and can also be used via PlaceHolderApi.

!!! note "PlaceHolder Api"
    As MCHockey supports multiple games per server, you need to specify the name of the game in external plugins. You can
    do this by appending the name of the game ``_game1`` ``_mygame``.
    This results into placeholders such as e.g. ``%mchockey_game_displayName_game1%``
    or ``%mchockey_game_blueScore_mygame%``. This is only relevant in external plugins. For placeholders in MCHockey, you
    can directly use the placeholders below.

| Game Context Placeholders           | Description                                                                                                   |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| %mchockey_game_name%               | Id of the game                                                                                                |
| %mchockey_game_displayName%        | DisplayName of the game                                                                                       |
| %mchockey_game_maxPlayers%         | Max amount of players who can join this game                                                                  |
| %mchockey_game_players%            | Current amount of players in this game                                                                        |
| %mchockey_game_redDisplayName%     | Name of team red                                                                                              |
| %mchockey_game_redScore%           | Score of the red team                                                                                         |
| %mchockey_game_redPlayers%         | Amount of players who are currently in the red team                                                           |
| %mchockey_game_redMaxPlayers%      | Max amount of players who can join the red team                                                               |
| %mchockey_game_blueDisplayName%    | Name of team blue                                                                                             |
| %mchockey_game_blueScore%          | Score of the blue team                                                                                        |
| %mchockey_game_bluePlayers%        | Amount of players who are currently in the blue team                                                          |
| %mchockey_game_blueMaxPlayers%     | Max amount of players who can join the blue team                                                              |
| %mchockey_game_time%               | Remaining time until the match ends                                                                           |
| %mchockey_game_lastHitPlayerName%  | Name of the player who was the last one to hit the ball, returns an empty text if no one has hit the ball yet |
| %mchockey_game_lastHitPlayerTeam%  | DisplayName of the team of the player who was the last one to hit the ball.                                   |
| %mchockey_game_state%              | Returns JOINABLE,RUNNING,DISABLED                                                                             |
| %mchockey_game_stateDisplayName%   | Returns the state color formatted from the language file                                                      |
| %mchockey_game_isEnabled%          | true if the game is enabled, false if not                                                                     |
| %mchockey_game_isJoinAble%         | true if the game is joinable, false if not                                                                    |
| %mchockey_game_remainingPlayers%   | Remaining amount of players required to start a match in minigame mode                                        |
| %mchockey_game_refereeDisplayName% | Name of team referee                                                                                          |

| Player Context Placeholders        | Description                                                    |
|------------------------------------|----------------------------------------------------------------|
| %mchockey_player_name%            | Name of the player during a MCHockey event e.g. scoring goal  |
| %mchockey_player_team%            | Name of the team the player is currently in: red, blue         |
| %mchockey_player_teamDisplayName% | Display name of the team the player is currently in.           |   
| %mchockey_player_isInGame%        | true if the player is in a game, false if not                  |
| %mchockey_player_isInTeamRed%     | true if the player is in a game and in team red, false if not  |
| %mchockey_player_isInTeamBlue%    | true if the player is in a game and in team blue, false if not |

| Stats Placeholders (Patreon Only)        | Description                                                                       |
|------------------------------------------|-----------------------------------------------------------------------------------|
| %mchockey_player_goals%                 | Amount of goals a player has scored                                               |
| %mchockey_player_goalsFull%             | Amount of goals a player has scored by playing full games.                        |
| %mchockey_player_goalsCurrent%          | Amount of goals a player has scored during the current game.                      |
| %mchockey_player_ownGoals%              | Amount of own goals a player has scored                                           |
| %mchockey_player_ownGoalsFull%          | Amount of own goals a player has scored by playing full games.                    |
| %mchockey_player_ownGoalsCurrent%       | Amount of own goals a player has scored during the current game.                  |
| %mchockey_player_totalGoals%            | Amount of goals and own goals a player has scored                                 |
| %mchockey_player_totalGoalsFull%        | Amount of goals and own goals a player has scored by playing full games.          |
| %mchockey_player_totalGoalsCurrent%     | Amount of goals and own goals a player has scored during the current game.        |
| %mchockey_player_games%                 | Amount of games a player has started playing                                      |
| %mchockey_player_gamesFull%             | Amount of games a player has fully played                                         |
| %mchockey_player_wins%                  | Amount of wins a player has got by playing                                        |
| %mchockey_player_losses%                | Amount of losses a player has got by playing                                      |
| %mchockey_player_draws%                 | Amount of draws a player has got by playing                                       |
| %mchockey_player_winrate%               | Ratio between amount of games a player has started playing and wins               |
| %mchockey_player_winrateFull%           | Ratio between amount of games a player has fully played and wins                  |
| %mchockey_player_goalsPerGame%          | Ratio between amount of games a player has started playing and scored goals       |
| %mchockey_player_goalsPerGameFull%      | Ratio between amount of games a player has fully played and scored goals          |
| %mchockey_player_ownGoalsPerGame%       | Ratio between amount of games a player has started playing and scored own goals   |
| %mchockey_player_ownGoalsPerGameFull%   | Ratio between amount of games a player has fully played and scored own goals      |
| %mchockey_player_totalGoalsPerGame%     | Ratio between amount of games a player has started playing and scored total goals |
| %mchockey_player_totalGoalsPerGameFull% | Ratio between amount of games a player has fully played and scored total goals    |

!!! note "LeaderBoard"
    Replace **top_1** with **top_2** or **top_3** etc. to build a leaderboard.

| LeaderBoard Placeholders (Patreon Only)                 | Description                                                                                  |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------|
| %mchockey_leaderboard_goals_name_top_1%                | The name of the player which has the most amount of scored goals                             |
| %mchockey_leaderboard_goals_value_top_1%               | The most amount of scored goals                                                              |
| %mchockey_leaderboard_goalsFull_name_top_1%            | The name of the player which has the most amount of scored goals by playing full games       |
| %mchockey_leaderboard_goalsFull_value_top_1%           | The most amount of scored goals by playing full games                                        |
| %mchockey_leaderboard_ownGoals_name_top_1%             | The name of the player which has the most amount of own goals                                |
| %mchockey_leaderboard_ownGoals_value_top_1%            | The most amount of own goals                                                                 |
| %mchockey_leaderboard_ownGoalsFull_name_top_1%         | The name of the player which has the most amount of own goals by playing full games          |
| %mchockey_leaderboard_ownGoalsFull_value_top_1%        | The most amount of own goals by playing full games                                           |
| %mchockey_leaderboard_totalGoals_name_top_1%           | The name of the player which has the most amount of total goals                              |
| %mchockey_leaderboard_totalGoals_value_top_1%          | The most amount of total goals                                                               |
| %mchockey_leaderboard_totalGoalsFull_name_top_1%       | The name of the player which has the most amount of total goals by playing full games        |
| %mchockey_leaderboard_totalGoalsFull_value_top_1%      | The most amount of total goals by playing full games                                         |
| %mchockey_leaderboard_games_name_top_1%                | The name of the player which has the most amount of joined games                             |
| %mchockey_leaderboard_games_value_top_1%               | The most amount of joined games                                                              |
| %mchockey_leaderboard_gamesFull_name_top_1%            | The name of the player which has the most amount of fully played games                       |
| %mchockey_leaderboard_gamesFull_value_top_1%           | The most amount of fully played games                                                        |
| %mchockey_leaderboard_wins_name_top_1%                 | The name of the player which has the most amount of wins                                     |
| %mchockey_leaderboard_wins_value_top_1%                | The most amount wins                                                                         |
| %mchockey_leaderboard_losses_name_top_1%               | The name of the player which has the most amount of losses                                   |
| %mchockey_leaderboard_losses_value_top_1%              | The most amount losses                                                                       |
| %mchockey_leaderboard_draws_name_top_1%                | The name of the player which has the most amount of draws                                    |
| %mchockey_leaderboard_draws_value_top_1%               | The most amount draws                                                                        |
| %mchockey_leaderboard_winrate_name_top_1%              | The name of the player which has the highest winrate                                         |
| %mchockey_leaderboard_winrate_value_top_1%             | The highest winrate                                                                          |
| %mchockey_leaderboard_goalsPerGame_name_top_1%         | The name of the player which has the most amount of goals per game                           |
| %mchockey_leaderboard_goalsPerGame_value_top_1%        | The most amount of goals per game                                                            |
| %mchockey_leaderboard_goalsPerGameFull_name_top_1%     | The name of the player which has the most amount of goals per game by playing full games     |
| %mchockey_leaderboard_goalsPerGameFull_value_top_1%    | The most amount of goals per game by playing full games                                      |
| %mchockey_leaderboard_ownGoalsPerGame_name_top_1%      | The name of the player which has the most amount of own goals per game                       |
| %mchockey_leaderboard_ownGoalsPerGame_value_top_1%     | The most amount of own goals per game                                                        |
| %mchockey_leaderboard_ownGoalsPerGameFull_name_top_1%  | The name of the player which has the most amount of own goals per game by playing full games |
| %mchockey_leaderboard_ownGoalsPerGameFull_value_top_1% | The most amount of own goals per game by playing full games                                  |


