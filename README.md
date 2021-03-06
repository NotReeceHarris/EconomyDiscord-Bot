# NotReeceHarris/🤖EcoBotV2 
###### _STILL IN DEVELOPMENT (DO NOT USE unless you are going to change the code)_

[![CodeQL](https://github.com/NotReeceHarris/EconomyDiscord-Bot/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/NotReeceHarris/EconomyDiscord-Bot/actions/workflows/codeql-analysis.yml) [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/NotReeceHarris/EconomyDiscord-Bot/blob/version-2/LICENSE) ![Version](https://img.shields.io/badge/Version-2.0-blue.svg) | [![Python](https://img.shields.io/badge/python-3.9-green.svg)](https://www.python.org/downloads/) [![DiscordPY](https://img.shields.io/badge/discord.py-1.6.0-blue.svg)](https://github.com/Rapptz/discord.py)
---

## SQLITE 3
This bot uses sqlite3 so unless you know how to query sql or modify the data changing users xp/level/money etc will come with difficulty
# Features
* Economy Features
  * Career
    - [x] Education
    - [ ] Jobs
  * Currency
    - [x] Wallet
    - [x] Bank
  * Crime system
    - [ ] Rob
    - [ ] Crime heat
    - [ ] Murder
  * <a href="#item-shop">Shop</a>
    - [x] <a href="#adding-to-the-item-shop">Items</a>
    - [x] 24 hour resets
* Moderation Systems
  * Utilities
    - [x] <a href="#ping">Ping</a>
  * Warning system
    - [ ] Roleplay Identity (Hidden within the roleplay aspect)
  * Activity System
    - [x] Message counter
    - [ ] Message logger
* Customization 
  - [x] <a href="#status-variables">Status variables</a>
  - [x] <a href="#level-variables">Level variables</a>
</samp>
# Customization

## Status variables

* `$total_members$`&nbsp;&nbsp;=> Total members
* `$total_guilds$`&nbsp;&nbsp;&nbsp;&nbsp;=> Total Servers
* `$prefix$`&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=> Prefix

### Examples <br>
`Over $total_members$ members!` <br>
<img src="https://cdn.discordapp.com/attachments/829487750809518081/829487787161681920/unknown.png" alt="Watching Over 3 members!"><br>
`$total_guilds$ servers!` <br>
<img src="https://cdn.discordapp.com/attachments/829487750809518081/829488805433966642/unknown.png" alt="Watching Over 2 servers!"><br>
`out for $prefix$` <br>
<img src="https://cdn.discordapp.com/attachments/829487750809518081/829489384033353758/unknown.png" alt="Watching out for !"><br>

## Level variables

* `$level$`&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=> Current Level
* `$name$`&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=> User Name
* `$last_level$`&nbsp;&nbsp;=> Last level

### Examples <br>
`Congrats on leveling up your now level $level$` <br>
<img src="https://cdn.discordapp.com/attachments/829487750809518081/829727402329505872/unknown.png" alt="Congrats on leveling up your now level 3"><br>
`$last_level$ >>> $level$` <br>
<img src="https://cdn.discordapp.com/attachments/829487750809518081/829727966786879498/unknown.png" alt="2 >>> 3"><br>

## Ping
Colour combos if your latency is within a range it will change the colour of the message<br>
`latency < 150 = Green`<br>
`150 < latency < 250 = Orange`<br>
`250 < latency = Red`<br>

# Item Shop

<img src="https://i.imgur.com/yWyKbCp.png" alt="Shop Embed"><br>

## adding to the item shop
withing the data folder you will find a json file called `items.json` add or modify items within there
example:
```python
{
   "id": 0,               # this has to be a unique integer 
   "name": "Apple",       # the name for the item
   "emoji": ":apple:",    # discord emojis only
   "price": {             # a price will be determined between 'start' and 'end' and a rarity will be given from this
      "start": 5,         # start price
      "end": 10           # end price
   }
}
```
