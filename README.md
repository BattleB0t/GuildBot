# GuildBot

> Hypixel guild bot.

Uses [discord.js-light](https://github.com/timotejroiko/discord.js-light) to communicate with [Discord](https://discord.com), and [Mineflayer](https://github.com/PrismarineJS/mineflayer) for [Hypixel](https://hypixel.net/) interactions.

```diff
- This application utilizes a non-vanilla Minecraft client to login to Hypixel, which could result in your Minecraft account being banned. Use at your own risk. -
```

## Setup
Coming Soon

## Commands

#### /help
List commands.

#### /link <username>
Link Minecraft and Discord account.

#### /check [username]
Check if a you/another user meet the guild requirements.

#### /apply
Apply to the guild.

#### /invite \<username\>
Invite user to the guild.

#### /promote \<username\>
Promote a user up one rank.

#### /demote \<username\>
Demote a user down one rank.

#### /relog
Relog the Minecraft bot.

## Configuration

### Options

#### `enforceNames` \<bool\>
Have the bot manage Discord nicknames.

#### `nameFormat` \<string\>
Formatting template for Discord nicknames.

Possible variables:
- `{name}` - Minecraft username
- `{cataLevel}` - Catacombs level
- `{skillAverage}` - Average skill level

#### `enableFragRun` \<bool\>
Enable frag run bot functionality.

#### `guildExclusive` \<bool\>
Restrict frag running availability to guild members.

#### `showJoinLeave` \<bool\>
Show player join/leave messages in the bridge channel.

#### `discord` \<string\>
Prefix for bridge messages sent from Discord.

#### `hypixel` \<string\>
Prefix for bridge messages sent from Hypixel.

#### `join` \<string\>
Prefix for bridge messages when a player joins.

#### `leave` \<string\>
Prefix for bridge messages when a player leaves.

#### `cataLevel` \<number\>
Required catacombs level to join the guild.

#### `secretCount` \<number\>
Required secret count to join the guild.

#### `skillAverage` \<number\>
Required skill average to join the guild.

#### `slayerEXP` \<number\>
Required slayer EXP to join the guild.

### Minecraft

#### `username` \<string\>
Minecraft account email.

#### `password` \<string\>
Minecraft account password.

#### `microsoftAuth` \<bool\>
Whether or not the account uses the new Microsoft authentication.

### Discord

#### `token` \<string\>
[Discord application](https://discord.com/developers/applications) token.

#### `status` \<string\>
Channel ID to place the bot/guild status message in.

#### `accountLink` \<string\>
Channel ID for account linking.

#### `chatBridge` \<string\>
Channel ID to use as the bridge between guild chat and Discord.

#### `applications` \<string\>
Channel ID for the application menu.

#### `roleMap` \<object[]\>
Map of guild roles to Discord roles for the bot to automatically apply. e.g

```json
"roleMap": [
  {
    "name": "Officer", // Hypixel Guild Role Name
    "roleId": "845901052313600020" // Discord Role ID
  },
  {
    "name": "default",
    "roleId": "845565580227379231"
  }
]
```

## Planned Features:
- Account Linking
- Frag Running
  - Restrictable to guild members
- Chat Bridge
- Automated Roles
- Automated Applications
