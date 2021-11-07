# Discord-Game-Show
A bot to handle an elimination round style game show in Discord!



## Game Flow 

* Virtual lobby (bot post in channel, opt in to game via emoji to message)
* After player threshold reached, game timer starts (2 minutes?)
* All players are allowed permissions to post in channel
* Play game start messages (rules, plot, etc)
* Pick first round game from pool of first rounds
* If player dies they are 'muted' from the channel
* Pick second round game from pool of second rounds
* If player dies they are 'muted' from the channel
* Pick third round game from pool of third rounds
* If player dies they are 'muted' from the channel
* Winner gets access to secret channel?
* Game restart (back to virtual lobby)


## Spontaneous Events 

* These happen between rounds at random and can be good or bad
* ex. player randomly explodes, gets revive perk, gun perk, etc
* Emojis in player nickname can indicate current inventory      
* Randomly selected by chance. The event type can be chosen from a pool with each event having a weight to control frequency.


## Player Object

* 2 types
* Game Player Object (Follows player throughout the game)
* Inventory? (power ups, perks, curses)
* Round Player Object (Ephemeral)
* Keep track of player data unique to that round 


## Round Structure

* Round Attributes
* Round ID (this will let us randomly choose a round type from a pool)
* Round difficulty (lets us classify round types into pools, rounds get harder as game progresses)
* Any other round specific data


## Game State

* In Game?
* Is Round or Event?
* living players
* dead players
* spectators
