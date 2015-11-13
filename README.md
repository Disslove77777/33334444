# <p align="center">merbot

<p align="center">**A Telegram Group Peace Keeper Bot**


**Merbot** is Telegram group guardian bot based on [telegram-bot](https://github.com/yagop/telegram-bot).

**Merbot** is dedicated as a group manager bot, so it's have no unnecessary plugins other than listed below. You can always add plugins as you need.

1. **Banhammer**. Plugin to manage bans, kicks and white/black lists.

  * Allow everybody on current chat to use the bot when whitelist mode is enabled.
  * Allow user to use the bot when whitelist mode is enabled.
  * Ban/unban user.
  * Enable or disable whitelist mode.
  * Kick user from chat and kicks it if joins chat again.
  * Kick user from chat group.
  * Remove chat from whitelist.
  * Remove user from whitelist.

2. **Channels**. Plugin to manage channels. Enable or disable channel.

  * Enable current channel.
  * Disable current channel.

3. **Group Manager**. Plugin to manage group chat.

  * Allow/disallow APIs bots to enter group.
  * Get or revoke invite link.
  * Lock/unlock group member.
  * Lock/unlock group name.
  * Lock/unlock group photo.
  * Read group description.
  * Read group rules.
  * Set group description.
  * Set group name.
  * Set group photo.
  * Set group rules.
  * Show group settings.

4. **Help**. Help plugin. Get info from other plugins.

  * Show all commands for every plugin.
  * Show Commands for that plugin.
  * Show list of plugins.

5. **Id**. Know your id or the id of a chat members.

  * Return the IDs of the `chat_id` members.
  * Return the IDs of the current chat members.
  * Return the member `@user_name` ID from the current chat.
  * Return your ID and the chat id if you are in one.
  * Search for users with `text` on `first_name`, `print_name` or `username` on current chat.

6. **Invite**. Invite other user to the chat group.

7. **Plugins**. Plugin to manage other plugins. Enable, disable or reload.

  * Disable plugin.
  * Disable plugin only this chat.
  * Enable plugin.
  * List all plugins.
  * Reloads all plugins.

8. **Version**. Shows bot version.

#### [Installation](https</code>://github.com/yagop/telegram-bot/wiki/Installation)

#### Dependencies

Tested on Ubuntu 14.04, for other OSs check out https://github.com/yagop/telegram-bot/wiki/Installation.

```bash
sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev libevent-dev make unzip git redis-server g++ libjansson-dev libpython-dev expat libexpat1-dev
```

#### Installation

After those dependencies, lets install the bot.

```bash
cd $HOME
git clone https://github.com/rizaumami/merbot.git
cd merbot
./merbot install
./merbot # Will ask you for a phone number & confirmation code.
```

If you use Ubuntu, which is use `upstart`, you can create an `upstart` script to manage `merbot`.

```bash
./merbot upstart
```

And then, start `merbot` by executing `sudo start merbot`. And stop `merbot` by `sudo stop merbot`.


#### Enable more [`plugins`](https</code>://github.com/rizaumami/merbot/tree/master/plugins)

See the plugins list with `!plugins` command.

Enable a disabled plugin by `!plugins enable [name]`.

Disable an enabled plugin by `!plugins disable [name]`.

Those commands require a privileged user, privileged users are defined inside `data/config.lua` (generated by the bot), stop the bot and edit if necessary.
