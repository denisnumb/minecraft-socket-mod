# minecraft-socket-mod

Mod for MineCraft, which implements a simple socket server for the interaction of third-party programs with the game server.

One of the options for using the functionality is to combine the MineCraft chat with the Discord server channel into one common chat.

![1](https://github.com/denisnumb/discord-minecraft-chat-socket/assets/61795655/33ec8918-5722-4b78-8e2a-f0da21900829)

The `minecraft_mod` directory contains the source code of the mod that implements a socket server that allows you to exchange messages with a Discord channel.

In the `discord_bot` directory there is a Discord bot that connects to the mod for messaging.

---

# Usage

1. [Download][1] and install **on the server** the latest version of the mod that matches the required version of the game. (The mod is only for the server side, no need to install it on the client!)
2. [Download][2] and install Python. Recommended version is not lower than `3.8`
3. Install the library to work with Discord:
```cmd
pip install py-cord
```
4. Start the server with the mod installed so that the mod configuration file is generated in the server directory
5. [Create a bot][3] and specify all the necessary parameters in the `discord_bot/config.py` file

If you run the bot and the server on the same device, then the IP address configuration data can be left untouched (leave `127.0.0.1`). 

Otherwise, you need to specify in the mod configuration the IP address of the server on which the Discord bot is running.  And in `config.py` specify the IP address of the MineCraft server.

---

The mod is under development and has practically not been tested, so the possibility of various bugs cannot be ruled out.

[1]: https://github.com/denisnumb/discord-minecraft-chat/releases
[2]: https://www.python.org/downloads/
[3]: https://discord.com/developers/docs/getting-started
