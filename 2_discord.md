# Documentació del Bot de Discord
![Logotip de Discord](https://commons.wikimedia.org/wiki/Special:FilePath/Discord_logo_simplified.svg)
[Logotip de discord](https://commons.wikimedia.org/wiki/Special:FilePath/Discord_logo_simplified.svg)
Pots registrar la teva aplicació al [Portal de Desenvolupadors de Discord](https://discord.com/developers/applications).

Per fer que el bot respongui, escoltem l'esdeveniment `messageCreate` i utilitzem el mètode `message.reply()`
```javascript
client.on('messageCreate', message => {
    if (message.content === 'ping') {
        message.reply('pong!');
    }
});
```