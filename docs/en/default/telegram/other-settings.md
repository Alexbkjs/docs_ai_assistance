---
type: page
title: Other Settings
seoTitle: Other Settings
seoDescription: Manage username display
slug: other-settings
order: 3
status: published
---


# Other Settings

## Manage username display

You can control how Discord usernames appear in Telegram using the "Show names of Discord users in Telegram" option. This allows you to customize how messages from the bot are displayed in Telegram.

By default, this option is disabled and messages appear as standard bot messages. If you have a support channel, for example, you may want messages to display text such as "New message from John."

To activate this option, follow these steps:

1.  Use the `/list` command to open the settings modal.
2.  Click on Settings → choose **Other settings** → **Show names of Discord users in Telegram**.
3.  Click **Enable** → **Edit message** → enter the text you want to display → click **Submit**.

![](https://cdn.heymantle.com/docs/screenshots/1af425b8-3bdd-4c75-ad2f-703cc39b70e9/other-settings_q72yy.png)

You can use the following variable to customize the message:

*   `{{displayName}}`: Displays the user's full name (e.g., John Smith).

![](https://cdn.heymantle.com/docs/screenshots/6858a54e-f04b-4913-a4f6-58accf804f8f/notification-settings-result_hp24ce.png)

This feature personalizes messages so they appear to come from a real person rather than a bot, helping to strengthen customer engagement, build user trust, and create a more natural communication experience.

## Re-create conversation thread

This option automatically creates a new thread when the current one has been inactive for an extended period. You can specify the inactivity period after which a new thread is created.

To activate this option, follow these steps:

1.  Use the `/list` command to open the settings modal.
2.  Click on Settings → choose **Other settings**.
3.  Find the **'Re-create conversation thread after'** button and select the time period: **24 hours** or **1 week**. Selecting **Never re-create** prevents new threads from being created, even after long inactivity.

![](https://cdn.heymantle.com/docs/screenshots/2c92cbc5-68eb-4ee3-8d70-bd217f47f51d/re-create-thread_ma99sh.png)

In the Settings section, you can also customize:

*   [New Message Notification](/telegram/new-message-notification)
*   [Message Forwarding](/telegram/message-forwarding)
*   [Message Filters](/telegram/message-filters)
*   [Greeting Message Notification](/telegram/greeting-message-notification)
*   [Forwarding Directions](/telegram/forwarding-directions)

## Suggested articles

*   [How to forward messages from a Telegram channel to Discord](/telegram/how-to-forward-messages-from-a-telegram-channel-to-discord)
*   [How to forward messages from a Telegram group to Discord](/telegram/how-to-forward-messages-from-a-telegram-group-to-discord)
