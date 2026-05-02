---
type: page
title: Troubleshooting connection issues
seoTitle: Troubleshooting connection issues
seoDescription: Unable to connect my bot to a Discord channel
slug: troubleshooting-connection-issues
order: 0
status: published
---

Articles on: [Telegram](/en/category/telegram-1urqa6t/)

# Troubleshooting connection issues

  

# Troubleshooting connection issues

  

****In this article:****

*   [Unable to connect my bot to a Discord channel](#1-unable-to-connect-my-bot-to-a-discord-channel)
*   [Messages from a Telegram group are not forwarded to a Discord thread/channel](#1-messages-from-a-telegram-group-are-not-forwarded-to-a-discord-thread-channel)
*   [Messages from a Telegram channel are not forwarded to a Discord channel/thread](#1-messages-from-a-telegram-channel-are-not-forwarded-to-a-discord-channel-thread)
*   [Unable to forward messages to a private Discord channel](#1-unable-to-forward-messages-to-a-private-discord-channel)
*   [Why doesn't Discord see my telegram message?](#1-why-doesnt-discord-see-my-telegram-message)

  

# ✔️ Unable to connect my bot to a Discord channel

  

If the connection to the channel fails, please ensure the bot has the necessary permissions in Discord: ****“View Channel”**** and ****“Manage Webhooks”****.

  

To check this, follow these steps:

  

*   View Channel: Server Settings -> Roles -> Edit -> Permissions -> View Channel.
*   Webhooks permissions: Server Settings -> Roles -> Edit -> Permissions -> Manage Webhooks.

  

Alternatively, you can assign ****"Administrator"**** permissions to the bot:

  

*   Admin permissions: Server Settings -> Roles -> Edit -> Permissions -> Administrator.

  

Additionally, the bot may require other permissions to function correctly, such as:

  

*   “Send Messages”
*   “Manage Channels”
*   “Attach Files”
*   “Create Public Threads”
*   “Send Messages in Threads”

  

****Note:**** There is no need to enable all of these permissions. It would be enough if you enable “Administrator” + “Manage Webhooks” permissions OR only the required additional permissions.

  

# ✔️ Messages from a Telegram group are not forwarded to a Discord thread/channel

  

The bot requires the appropriate permissions to forward messages from the Telegram group to the Discord thread and channels.

  

****Forward to threads****

  

Please make sure the bot has “View Channel”, “Send Messages”, “Create Public Threads”, “Send Messages in Threads”, or only “Administrator” permissions.

  

Check this by following these steps:

  

*   Server settings -> Roles -> Edit -> Permissions -> Select the required permissions.

  

****Forward to channels****

  

Please make sure the bot has “View Channel”, “Manage Channel”, “Send Messages”, “Manage Webhooks”, or only “Administrator” permissions.

  

Check this by following these steps:

  

*   Server settings -> Roles -> Edit -> Permissions -> Select the required permissions.

  

# ✔️ Messages from a Telegram channel are not forwarded to a Discord channel/thread

  

The bot requires the appropriate permissions to forward messages from the Telegram channel to the Discord channel.

  

Please make sure the bot has “View Channel”, “Manage Channels”, “Send Messages”, “Manage Webhooks”, or “Administrator” permissions.

  

If the above permissions are not granted, the bot will not be able to create a channel on your server.

  

Check permissions by following these steps:

  

*   Server settings -> Roles -> Edit -> Permissions -> Select the required permissions.

  

# ✔️ Unable to forward messages to a private Discord channel

  

First of all you need to add the bot as a channel member in the channel's permissions.

  

*   Edit Channel -> Permissions -> Added as a member (or in Role)

  

Also, please ensure the bot has the necessary permissions: “View Channel”, “Send Messages”, “Create Public Threads”, “Send Messages in Threads”, “Administrator”. You can do this by following these steps:

  

*   Permissions: Server Settings -> Roles - > Edit -> Permissions -> Select the required permissions.

  

# ✔️ Why doesn't Discord see my Telegram message?

  

Discord doesn't see the message because the bot is not added as an administrator to the channel or group in Telegram. Read these articles, to learn more about how to forward messages from Telegram group or channel to Discord:

  

*   [How to forward messages from a Telegram group to Discord?](/how-to-forward-messages-from-a-telegram-group-to-discord)
*   [How to forward messages from a Telegram channel to Discord?](/how-to-forward-messages-from-a-telegram-channel-to-discord)

  

Updated on: 05/08/2025