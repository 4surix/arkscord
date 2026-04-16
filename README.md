# Arkscord
**ArkSc**ript + Di**scord** = **Arkscord**   
Module used to interact with the [Discord](https://discord.com/) API using [ArkScript](https://github.com/ArkScript-lang/Ark) language.

# Exemple

```clojure
(import arkscord.client)

(let token "TOKEN-BOT-DISCORD")
(let bot (client:createBot token))

(bot.listenChannelsIds [
    "<CHANNEL-ID>"
])

(bot.onMessage (fun (message) {
  (print message.author.name ": " message.content) }))

(bot.run)
```