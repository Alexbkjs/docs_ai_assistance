---
type: page
title: How to forward messages from a Telegram channel to Discord?
seoTitle: How to forward messages from a Telegram channel to Discord?
seoDescription: Create a Telegram bot and connect it to the Telegram channel
slug: how-to-forward-messages-from-a-telegram-channel-to-discord
order: 1
status: published
---


# Forward messages from the Telegram channel

## Create a Telegram bot and connect it to the Telegram channel

1.  Create your Telegram bot (if you already have a bot, use it to connect to the Telegram channel). You can do this using the [BotFather](https://t.me/BotFather) bot on Telegram. For more details, refer to [this article](/telegram/getting-started-with-telegram-bot).
2.  Add the Telegram bot to the Telegram channel:

*   Open your Telegram channel → click on its name → Subscribers → click **Add subscribers** and add the bot as a subscriber.
*   A modal window will appear allowing you to add the bot as an admin → click **Add as admin**.

Note: Granting the bot admin rights allows it to send messages.

![](https://cdn.heymantle.com/docs/screenshots/96b5592a-5164-4d92-bfca-53ef5f34567e/telegram-channel-settings_1cn444p.png)

Note: Go to the Admin Rights section and ensure the bot has the "Manage Messages" permission.

## Connect the Telegram bot to Discord

1.  Go back to [BotFather](https://t.me/BotFather) and copy the bot's token (if you already have a bot, use its existing token).
2.  Open the Discord channel where you want to connect the bot → type the `/connect` command in the text field and send it.
3.  Paste the token in the field that appears and click **Submit**.

**Note:** For more details on the difference between forwarding to channels and threads, see [Message Forwarding](/telegram/message-forwarding).

**Important:** If the connection fails, ensure the bot has the necessary permissions in Discord:

*   Admin permissions: Server Settings → Roles → Edit → Permissions → Administrator.
*   Webhook permissions: Server Settings → Roles → Edit → Permissions → Manage Webhooks.

While the bot is connected, you can manage its settings. Use the `/list` command to open the settings window and click **Settings**. For example, you can set up where to forward messages from Telegram — to [Discord channels or threads](/telegram/message-forwarding). You can also manage:

*   [New Message Notification](/telegram/new-message-notification)
*   [Message Filters](/telegram/message-filters)
*   [Greeting Message Notification](/telegram/greeting-message-notification)
*   [Other Settings](/telegram/other-settings)

Take a moment to explore and adjust any settings you need.

If you also need to forward messages from a Telegram group to Discord, see [How to forward messages from a Telegram group to Discord?](/telegram/how-to-forward-messages-from-a-telegram-group-to-discord)
