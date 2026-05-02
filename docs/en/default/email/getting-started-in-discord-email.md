---
type: page
title: Getting started in Discord Email
seoTitle: Getting started in Discord Email
seoDescription: Connect Email bot to the Discord channel
slug: getting-started-in-discord-email
order: 5
status: published
---


# Quick start in Email bot

<iframe type="text/html" width="560" height="349" src="https://www.youtube.com/embed/Kz8jVwJlIxM?rel=0" loading="lazy" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; border: 0px;"></iframe>

## Connect Email bot to the Discord channel

Invite the [Discord Email Bot](https://top.gg/bot/1106165894859735070) and follow these steps:

1.  Open the channel where you want to use the bot, type `/connect` in the message field, and press Enter.
2.  The bot will instantly create a **unique email address** for that channel. Any emails sent to this address will appear directly in the channel.
3.  Send a test message from your personal email, and you'll see it appear in Discord within moments.

Note that there are **two modes** for how messages are displayed in Discord:

*   Subject only
*   Subject + preview of the message (if previously [enabled](/email/email-preview-in-message))

![](https://cdn.heymantle.com/docs/screenshots/d32f558b-0956-4e3c-9ba8-330efd21835e/test-messages-discord_1hw3ly.png)

You can also **attach files, images, and other media** to the message — they will be delivered to the channel as well.

![](https://cdn.heymantle.com/docs/screenshots/67e5a56d-a03a-4aba-afb1-42b4fe6a176e/test-message-with-image_g26hpb.png)

Want to use the bot in multiple channels? Simply run the `/connect` command in each one. Every channel gets its own unique email address, so you can create as many integrations as you need.

## Available commands

1.  `/connect`

Connect a unique email address to your Discord channel. You can use this address to subscribe to newsletters, alerts, or other important notifications.

![](https://cdn.heymantle.com/docs/screenshots/974bca54-eefa-44fd-9288-8cd89c609be5/the-connect-command_zvgoue.png)

2.  `/list`

Displays details about your connected email, along with setup options and email statistics.

You'll also see **interaction statistics** for two timeframes:

*   Last 30 days – total number of emails received in the past 30 days.
*   Billing period – total number of emails received since the start of your current billing cycle.

**Additional options** available in this menu:

*   Disconnect – remove the bot from the channel.
*   Settings – view and adjust available bot settings.
*   View email statistics – check your current subscription, monthly limits, and rate limits.

![](https://cdn.heymantle.com/docs/screenshots/ab44ed04-1608-4f07-aa2b-6b2050977418/the-list-command_1yumpu4.png)

3.  `/help`

Get help with bot commands and useful links to the Help Guide or support team.

## Advanced setup

Use the `/list` command and click Settings to customize your emails.

For example, you can include a [web version](/email/web-version-of-emails) of the email directly within the main message. The bot also allows you to include a [preview of the email content](/email/email-preview-in-message), enable or disable the [Reply option](/email/message-reply-option), and adjust the email name and avatar via [Email Personalization](/email/email-personalization).

## Limitations

Note that the following limits apply to emails sent to this integration:

*   The combined headers and body of an email cannot exceed 1 MB.
*   When combined with attachments, an email cannot exceed 30 MB.
*   A maximum of 20 attachments per email is allowed.

## Useful links

*   Check our [FAQ](/email/frequently-asked-questions) if you have questions about the bot.
*   Read this article if your [emails aren't showing up in the channel](/email/troubleshooting-why-aren-t-emails-showing-up-in-the-channel).
