# HC Alert
Hardcore Alert
- Discord Bot to Alert on World of Warcraft Classic Hardcore Deaths and Level Up  

Pictures are worth a thousand words so here is what it looks like:  

![](https://raw.githubusercontent.com/ninthwalker/HCAlert/main/screenshots/hcalert_example.png)  

Here is the link to add the HC Alert bot to your own discord server:  
[HC Alert Discord Bot](https://discord.com/api/oauth2/authorize?client_id=1145545491237572688&permissions=18432&scope=bot)    
  
Here is the Support Discord for help or more info.  
[HC Alert Support](https://discord.gg/X6eZCexAFz)    
  
Stay Alert, Stay Alive!  

#### Bot Commands

**Primary slash command: `/hcalert`**

**Secondary optional settings:**  
- **Alert Type:** Death Only, Level Up Only, Death & Level Up.  
- **Minimum Level:** Minimum char level before any alert will occur. Min is 10. Default is 10. (Blizz does not record char level before that)
- **Level Increment:** For Level Up alerts, set this for how often to be alerted.  
ie: If set to 2, alerts will go out for lvl's 10, 12, 14.. Default is 2.
- **Guild:** Select 'Yes' if this is a guild and not a character.

#### Subcommands:
- **Add**  
Adds a new character or guild for death or level up alerts. Realm & Char/Guild name are required, other fields are optional.
`<realm> <char/guild name> <alert type> <Min. char level>[10 min, default: 10] <level increment>[default: 2] <guild>`
- **Remove**  
Removes a char or guild from alerting
`<select realm> <char/guild name> <guild>`
- **Set**  
Discord Server Bot Settings. Use to set channel for bot to post to, as well as default options. Default options are used when those same options are not specified when adding a character.  
`<channel to post to> <alert type> <Min. char level>[10 min, default: 10] <level increment>[default: 2]`
- **Leaderboard**  
Shows all current character levels
- **List**  
Outputs all configured alerts for this discord server. Useful to see who you already added or who you want to remove.
- **Check**  
Manually check a characters current level and status
- **Help**  
List command informatin for the bot
​
If you are feeling generous or would like to support some of my coding projects, you can contribute via [Github Sponsors](https://github.com/sponsors/ninthwalker) ☕
