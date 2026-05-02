---
type: page
title: How to forward messages from a Telegram group to Discord?
seoTitle: How to forward messages from a Telegram group to Discord?
seoDescription: Create a Telegram bot and connect it to the Telegram group
slug: how-to-forward-messages-from-a-telegram-group-to-discord
order: 2
status: published
---

Articles on: [Telegram](/en/category/telegram-1urqa6t/)

# How to forward messages from a Telegram group to Discord?

  

# Forward messages from the Telegram group

  

****In this article:****

*   [Create a Telegram bot and connect it to the Telegram group](#1-create-a-telegram-bot-and-connect-it-to-the-telegram-group)
*   [Connect Telegram bot to Discord](#1-connect-telegram-bot-to-discord)

  

# ✔️ Create a Telegram bot and connect it to the Telegram group

  

1.  Create your Telegram bot (if you already have a bot, use it to connect to the Telegram group). You can do this by using the [BotFather](https://t.me/BotFather) bot on Telegram. For more detailed information, refer to [this article](/getting-started-with-telegram-bot).
2.  Add the Telegram Bot to the Telegram group:

  

*   Open your Telegram group -> click on the group title and click ****Add Members**** and add the created bot as a member.
*   Press on the bot and click on ****Promote to admin**** -> click on the checkmark in the top-right corner.

  

Note: Providing the bot with admin rights enables it to send messages.

  

![](https://cdn.heymantle.com/docs/screenshots/ea07a8f0-66c8-4c99-a557-521394badc49/telegram-group_1oj7zcv.png)

  

# ✔️ Connect Telegram bot to Discord

  

1.  Go back to the [BotFather](https://t.me/BotFather) and copy the bot’s token (if you already have a bot, use its token to connect it to Discord).
2.  Open the Discord channel where you want to connect the bot -> type the `/connect` command in the text field and send this message.
3.  Paste the token in the appeared field and click ****Submit****.

  

You can find more detailed information about the difference in forwarding to channels and threads in the article - [Message Forwarding](/message-forwarding).

  

****Important:**** If the connection to the channel fails, please ensure the bot has the necessary admin permissions or permission to manage webhooks in Discord. To check this, follow these steps:

  

*   Admin permissions: Server Settings -> Roles -> Edit -> Permissions -> Administrator.
*   Webhooks permissions: Server Settings -> Roles -> Edit -> Permissions -> Manage Webhooks.

  

While the bot is connected, you can manage its settings. Just use the `/list` command to open the settings window and click ****Settings****. For example, you can setup where to forward messages from Telegram: to [Discord channels or threads](/message-forwarding). There you can also manage:

  

*   [New Message Notification](/new-message-notification)
*   [Message Filters](/message-filters)
*   [Greeting Message Notification](/greeting-message-notification)
*   [Other Settings](/other-settings)

  

Take a moment to explore and make any settings you need.

  

Also, we recommend you to check this article if you need forward messages from a Telegram channel to Discord - [How to forward messages from a Telegram channel to Discord?](/how-to-forward-messages-from-a-telegram-channel-to-discord)

Updated on: 21/05/2025