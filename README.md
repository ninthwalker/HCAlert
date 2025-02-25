# HC Alert
**Discord Bot to Alert on World of Warcraft Classic Hardcore Deaths and Level Up**  

Pictures are worth a thousand words so here is what it looks like:  

![](https://raw.githubusercontent.com/ninthwalker/HCAlert/main/screenshots/hcalert_example.png)  

### Installation
Here is the link to add the HC Alert bot to your own discord server:  
[HC Alert Discord Bot](https://discord.com/api/oauth2/authorize?client_id=1145545491237572688&permissions=18432&scope=bot)  

Permissions needed for the bot on the channel you set it to post in:  
```
Send Messages
Embed Links
```
  
Only requirement is for the server owner/admin to use the  `/hcalert set` command to configure the channel for the bot to post to. The other options for set are optional. Most of the /hcalert commands are self-explanatory or use `/hcalert help` for additional explanations.  

### Support  
Here is the Support Discord for help or more info:    
[HC Alert Support](https://discord.gg/X6eZCexAFz)    
  
Stay Alert, Stay Alive!  

## Bot Commands

**Primary slash command: `/hcalert`**

**Secondary optional settings:**  
- **Alert Type:** Death Only, Level Up Only, Death & Level Up. [Default: Death Only]
- **Minimum Level:** Minimum char level before any alert will occur. Min is 10. [Default is 10 for chars and 20 for guilds]
- **Level Increment:** For Level Up alerts, set this for how often to be alerted. [Default: 3]  
ie: If set to 2, alerts will go out for lvl's 10, 12, 14..
- **Guild:** Select `Yes` if this is a guild and not a character.

### Subcommands:
- **Add**  
Adds a new character or guild for death or level up alerts. Realm & Char/Guild name are required, other fields are optional.
`<realm> <char/guild name> <alert type> <Min. char level>[10 min, default: 10] <level increment>[default: 3] <guild>`
- **Remove**  
Removes a char or guild from alerting
`<select realm> <char/guild name> <guild>`
- **Set**  
Discord Server Bot Settings. Use to set channel for bot to post to, as well as default options. Default options are used when those same options are not specified when adding a character.  
`<channel to post to> <alert type> <Min. char level>[10 min, default: 10] <level increment>[default: 3]`
- **Leaderboard**  
Shows all current character levels
- **List**  
Outputs all configured alerts for this discord server. Useful to see who you already added or who you want to remove.
- **Check**  
Manually check a characters current level and status
- **Help**  
List command informatin for the bot

### Known Issues/Limitations
- Blizzard only updates on character logout
- Blizzard only tracks characters that are level 10+
- Guild limitations: Due to Blizzard API limits, guild minimum level is set to 20, there can only be one guild per discord server, and guilds are checked once an hour.
- If you die, logout, immediately delete and create a character with the same name before the API gets checked, the bot will not know of the death or be able to report it. Will think you are still whatever level you died at. To fix, use the `/hcalert remove` command to remove the character and then add it again. Alternatively, wait until you reach the level you died at again and the bot will resume reporting.  

If you are feeling generous or would like to support some of my coding projects, you can contribute via [Github Sponsors](https://github.com/sponsors/ninthwalker) ☕
