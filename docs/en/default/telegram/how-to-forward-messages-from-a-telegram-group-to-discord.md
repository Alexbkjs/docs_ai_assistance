---
type: page
title: How to forward messages from a Telegram group to Discord?
seoTitle: How to forward messages from a Telegram group to Discord?
seoDescription: Create a Telegram bot and connect it to the Telegram group
slug: how-to-forward-messages-from-a-telegram-group-to-discord
order: 2
status: published
---


# Forward messages from the Telegram group

## Create a Telegram bot and connect it to the Telegram group

1.  Create your Telegram bot (if you already have a bot, use it to connect to the Telegram group). You can do this using the [BotFather](https://t.me/BotFather) bot on Telegram. For more details, refer to [this article](/telegram/getting-started-with-telegram-bot).
2.  Add the Telegram bot to the Telegram group:

*   Open your Telegram group → click on the group title → click **Add Members** and add the bot as a member.
*   Press on the bot and click **Promote to admin** → click the checkmark in the top-right corner.

Note: Granting the bot admin rights allows it to send messages.

![](https://cdn.heymantle.com/docs/screenshots/ea07a8f0-66c8-4c99-a557-521394badc49/telegram-group_1oj7zcv.png)

## Connect the Telegram bot to Discord

1.  Go back to [BotFather](https://t.me/BotFather) and copy the bot's token (if you already have a bot, use its existing token).
2.  Open the Discord channel where you want to connect the bot → type the `/connect` command in the text field and send it.
3.  Paste the token in the field that appears and click **Submit**.

For more details on the difference between forwarding to channels and threads, see [Message Forwarding](/telegram/message-forwarding).

**Important:** If the connection fails, ensure the bot has the necessary permissions in Discord:

*   Admin permissions: Server Settings → Roles → Edit → Permissions → Administrator.
*   Webhook permissions: Server Settings → Roles → Edit → Permissions → Manage Webhooks.

While the bot is connected, you can manage its settings. Use the `/list` command to open the settings window and click **Settings**. For example, you can set up where to forward messages from Telegram — to [Discord channels or threads](/telegram/message-forwarding). You can also manage:

*   [New Message Notification](/telegram/new-message-notification)
*   [Message Filters](/telegram/message-filters)
*   [Greeting Message Notification](/telegram/greeting-message-notification)
*   [Other Settings](/telegram/other-settings)

Take a moment to explore and adjust any settings you need.

If you also need to forward messages from a Telegram channel to Discord, see [How to forward messages from a Telegram channel to Discord?](/telegram/how-to-forward-messages-from-a-telegram-channel-to-discord)
