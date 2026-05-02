---
type: page
title: Troubleshooting connection issues
seoTitle: Troubleshooting connection issues
seoDescription: Unable to connect my bot to a Discord channel
slug: troubleshooting-connection-issues
order: 0
status: published
---


# Troubleshooting connection issues

## Unable to connect my bot to a Discord channel

If the connection fails, ensure the bot has the necessary permissions in Discord: **"View Channel"** and **"Manage Webhooks"**.

To check this, follow these steps:

*   View Channel: Server Settings → Roles → Edit → Permissions → View Channel.
*   Webhook permissions: Server Settings → Roles → Edit → Permissions → Manage Webhooks.

Alternatively, you can assign **"Administrator"** permissions to the bot:

*   Admin permissions: Server Settings → Roles → Edit → Permissions → Administrator.

The bot may also require these additional permissions to function correctly:

*   "Send Messages"
*   "Manage Channels"
*   "Attach Files"
*   "Create Public Threads"
*   "Send Messages in Threads"

**Note:** You do not need to enable all of these. Enabling "Administrator" + "Manage Webhooks" is sufficient, or you can enable only the specific additional permissions you need.

## Messages from a Telegram group are not forwarded to a Discord thread or channel

The bot requires the appropriate permissions to forward messages from the Telegram group to Discord threads and channels.

**Forward to threads**

Ensure the bot has "View Channel", "Send Messages", "Create Public Threads", "Send Messages in Threads", or simply "Administrator" permissions.

To check these:

*   Server settings → Roles → Edit → Permissions → Select the required permissions.

**Forward to channels**

Ensure the bot has "View Channel", "Manage Channel", "Send Messages", "Manage Webhooks", or simply "Administrator" permissions.

To check these:

*   Server settings → Roles → Edit → Permissions → Select the required permissions.

## Messages from a Telegram channel are not forwarded to a Discord channel or thread

The bot requires the appropriate permissions to forward messages from the Telegram channel to Discord.

Ensure the bot has "View Channel", "Manage Channels", "Send Messages", "Manage Webhooks", or "Administrator" permissions.

Without these permissions, the bot will not be able to create a channel on your server.

To check permissions:

*   Server settings → Roles → Edit → Permissions → Select the required permissions.

## Unable to forward messages to a private Discord channel

First, add the bot as a channel member in the channel's permissions:

*   Edit Channel → Permissions → Added as a member (or in a Role)

Also ensure the bot has the necessary permissions: "View Channel", "Send Messages", "Create Public Threads", "Send Messages in Threads", "Administrator". To do this:

*   Permissions: Server Settings → Roles → Edit → Permissions → Select the required permissions.

## Why doesn't Discord receive my Telegram message?

Discord does not receive the message because the bot has not been added as an administrator to the channel or group in Telegram. See these articles to learn more about forwarding messages from Telegram to Discord:

*   [How to forward messages from a Telegram group to Discord?](/telegram/how-to-forward-messages-from-a-telegram-group-to-discord)
*   [How to forward messages from a Telegram channel to Discord?](/telegram/how-to-forward-messages-from-a-telegram-channel-to-discord)
