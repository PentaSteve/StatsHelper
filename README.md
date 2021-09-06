StatsHelper
-------

Statistics assistant   [MCDReforged](https://github.com/Fallen-Breath/MCDReforged) Plug-in, you can query/rank/use the scoreboard to list all kinds of statistical information.

Applicable version: 1.13 or above server 

# Format description 

`!!stats` Display help information 

`!!stats save` <code name> <statistics category> <statistics content> <title> save a quick scoreboard 

`!!stats del` <codename> remove a quick scoreboard 

`!!stats list` List saved quick scoreboards 
 
`!!stats query` <player> <statistics category> <statistics content> [<-uuid>] [<-tell>]

`!!stats query` <player> <name> [<-uuid>] [<-tell>]

`!!stats rank` <Statistics category> <Statistics content> (-bot) [<-tell>]

`!!stats rank` <Substitute name> (-bot) [<-tell>]

`!!stats scoreboard` <Statistics category> <Statistics content> (title) (-bot)

`!!stats scoreboard` <name> shows a quick scoreboard 

`!!stats scoreboard show` Show the scoreboard of the plugin 

`!!stats scoreboard hide` Hide the scoreboard of this plugin 

# Parameter Description 

<Statistics category>: killed, killed_by, dropped, picked_up, used, mined, broken, crafted, custom, killed, killed_by The <statistics> is [biological id]
 
picked_up, used, mined, broken, crafted The <statistics> is the item/block id 

custom <Statistics> See the json file of statistical information for details, or [MC Wiki](https://minecraft.fandom.com/zh/wiki/%E7%BB%9F%E8%AE%A1%E4%BF%A1%E6%81%AF)

The above content does not need to be prefixed with minecraft

[<-uuid>]: Replace the player name with uuid; (-bot): Count bot and cam; [<-tell>]: Only visible to yourself

# example

`!!stats save fly custom aviate_one_cm aviate list`

`!!stats query Fallen_Breath used water_bucket`

`!!stats rank custom time_since_rest -bot`

`!!stats scoreboard mined stone dig stone list`
