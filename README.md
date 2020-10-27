# Arkscord
**ArkSc**ript + Di**scord** = **Arkscord**  
Module servant à interagir avec l'API [Discord](https://discord.com/) en langage [ArkScript](https://github.com/ArkScript-lang/Ark).    

# Aperçu
```clojure
(let token "TOKEN-BOT-DISCORD")
(let bot (create-bot token))
(bot.listen-channels-ids [
    "513284461555744768"
])
(bot.on-message (fun (message) {
    (print message.author.name ": " message.content)
}))
(bot.run)
```