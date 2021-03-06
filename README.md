# resolve-it
Resolve emoji, member, guild, channel with their id and obtain them with 100% of success.

>Working with `DJS v12 & v13`
>and usable with `Typescript`

## Usage

> the resolver methods always take 2 parameters and are used with `await` key cause their return are  asynchronous.

```javascript
import * as Discord from "discord.js"

import { Resolving } from "resolvinger"
// OR
const Resolving = require("resolvinger")
// resolves a member
await Resolving.resolveMember(guild, memberID)
// resolves a channel
await Resolving.resolveChannel(guild, channelID)
// resolves an emoji
await Resolving.resolveEmoji(guild, emojiID)
// resolves an guild
await Resolving.resolveGuild(client, guildID)

// For example: 

<Client>.on("messageCreate", async message => {
await Resolving.resolveMember(message.guild, message.member.id)
// result: The GuildMember that wrote a message.
})
  
```
