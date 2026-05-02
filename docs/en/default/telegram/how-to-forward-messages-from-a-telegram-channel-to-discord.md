---
type: page
title: How to forward messages from a Telegram channel to Discord?
seoTitle: How to forward messages from a Telegram channel to Discord?
seoDescription: Create a Telegram bot and connect it to the Telegram channel
slug: how-to-forward-messages-from-a-telegram-channel-to-discord
order: 1
status: published
---

Articles on: [Telegram](/en/category/telegram-1urqa6t/)

# How to forward messages from a Telegram channel to Discord?

# Forward messages from the Telegram channel

****In this article:****

*   [Create a Telegram bot and connect it to the Telegram channel](#1-create-a-telegram-bot-and-connect-it-to-the-telegram-channel)
*   [Connect Telegram bot to Discord](#1-connect-telegram-bot-to-discord)

# ✔️ Create a Telegram bot and connect it to the Telegram channel

1.  Create your Telegram bot (if you already have a bot, use it to connect to the Telegram group). You can do this by using the [BotFather](https://t.me/BotFather) bot on Telegram. For more detailed information, refer to [this article](/getting-started-with-telegram-bot).
2.  Add the Telegram Bot to the Telegram channel:

*   Open your Telegram channel -> click on its name -> Subscribers -> click ****Add subscribers**** and add the created bot as a subscriber.
*   You will see a modal window that allows you to add a bot as admin -> click on ****Add as admin****.

Note: Providing the bot with admin rights enables it to send messages.

![](https://cdn.heymantle.com/docs/screenshots/96b5592a-5164-4d92-bfca-53ef5f34567e/telegram-channel-settings_1cn444p.png)

Note: Go to the Admin Rights section and ensure that the bot has the “Manage Messages” permission.

# ✔️ Create a Telegram bot and connect it to the Telegram channel

1.  Go back to the [BotFather](https://t.me/BotFather) and copy the bot’s token (if you already have a bot, use its token to connect it to Discord).
2.  Open the Discord channel where you want to connect the bot -> type the `/connect` command in the text field and send this message.
3.  Paste the token in the appeared field and click ****Submit****.

****Note:**** You can find more detailed information about the difference in forwarding to channels and threads in the article - [Message Forwarding](/message-forwarding).

****Important:**** If the connection to the channel fails, please ensure the bot has the necessary admin permissions or permission to manage webhooks in Discord. To check this, follow these steps:

*   Admin permissions: Server Settings -> Roles -> Edit -> Permissions -> Administrator.
*   Webhooks permissions: Server Settings -> Roles -> Edit -> Permissions -> Manage Webhooks.

While the bot is connected, you can manage its settings. Just use the `/list` command to open the settings window and click ****Settings****. For example, you can setup where to forward messages from Telegram: to [Discord channels or threads](/message-forwarding). There you can also manage:

*   [New Message Notification](/new-message-notification)
*   [Message Filters](/message-filters)
*   [Greeting Message Notification](/greeting-message-notification)
*   [Other Settings](/other-settings)

Take a moment to explore and make any settings you need.

Also, we recommend you to check this article if you need forward messages from a Telegram group to Discord - [How to forward messages from a Telegram group to Discord?](/how-to-forward-messages-from-a-telegram-group-to-discord)

Updated on: 11/12/2025