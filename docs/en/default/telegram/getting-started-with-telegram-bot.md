---
type: page
title: Getting started with Telegram bot
seoTitle: Getting started with Telegram bot
seoDescription: "To connect Telegram bot to your Discord channel, follow these steps:"
slug: getting-started-with-telegram-bot
order: 10
status: published
---


# Connect Telegram

<iframe type="text/html" width="560" height="349" src="https://www.youtube.com/embed/-Ll_-XG9i9w?rel=0" loading="lazy" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; border: 0px;"></iframe>

To connect the [Telegram bot](https://top.gg/bot/1123949801613049866) to your Discord channel, follow these steps:

1.  Create your Telegram bot (if you already have a bot, skip to the next step).

Go to Telegram and open [BotFather](https://t.me/BotFather). Here you can create and manage your Telegram bots.

Click **Start** → select the `/newbot` command from the list. Choose a name for your bot and copy the provided token.

**Important:** You can forward messages from Telegram channels and groups to Discord. When you add a bot to a group or channel in Telegram, you must grant it admin rights so the bot can view, send, edit, and delete messages.

2.  Open your Discord server and run the `/connect` command in any Discord channel where you want to connect the bot, then provide the token.

After connecting, conversations from your Telegram bot are forwarded to the connected Discord channel as public threads. All replies in those threads are forwarded back to the Telegram chat.

![](https://cdn.heymantle.com/docs/screenshots/065a1195-678f-47a3-82cc-c43dd8240c8c/telegram-bot_7d7aj7.png)

To set up the application according to your needs, use the **Settings** section. Send the `/list` command in the channel where you connected the app, then click **Settings**.

In the Settings section, you can also customize:

*   [New Message Notification](/telegram/new-message-notification)
*   [Message Forwarding](/telegram/message-forwarding)
*   [Message Filters](/telegram/message-filters)
*   [Greeting Message Notification](/telegram/greeting-message-notification)
*   [Other Settings](/telegram/other-settings)

## Suggested articles

*   [Welcome to Telegram bot](/telegram/welcome-to-telegram-bot)
*   [Frequently asked questions](https://help.devit.software/en/article/frequently-asked-questions-telegram-c5fl8s/)
