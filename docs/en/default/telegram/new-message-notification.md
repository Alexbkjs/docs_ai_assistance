---
type: page
title: New Message Notification
seoTitle: New Message Notification
seoDescription: This option allows you to customize messages for users, groups, or channels. You can personalize them to create a more welcoming and pleasant experience for your audience.
slug: new-message-notification
order: 8
status: published
---


# Manage New Message Notification

This option allows you to customize notifications for users, groups, or channels. You can personalize them to create a more welcoming experience for your audience.

To customize a notification, follow these steps:

1.  Use the `/list` command to open the settings modal.
2.  Click on **Settings** → choose a settings category → **New Message Notification**.
3.  Select the notification you want to edit and click **Edit notification**.

![](https://cdn.heymantle.com/docs/screenshots/e25c04e9-075d-4a3e-9952-8bfe0fcb756e/edit-message-notification_tuc7h7.png)

In the window that appears, enter the message text you want to display and click **Submit**.

You can use the following variables to customize your notification:

*   `{{fullName}}`: Displays the user's full name (e.g., **John Smith**).

Note: This does not create a link to the user's Telegram chat.

*   `{{userName}}`: Displays the user's username as a clickable link (e.g., **@john\_smith**).

Note: Not all users have a username, but every user has a full name.

*   `{{name}}`: Automatically uses either `{{fullName}}` or `{{userName}}`, depending on availability. If a username exists, it is used; otherwise, the full name is displayed.

![](https://cdn.heymantle.com/docs/screenshots/514917eb-4181-495a-a63d-33511fa20798/new-message_t98da2.png)

Note: Telegram supports public and private groups and channels. Public groups include links when the `{{userName}}` or `{{name}}` variables are used. For private groups or channels, only the group name is displayed — no link is included, regardless of the variable assigned.

In the Settings section, you can also customize:

*   [Message Forwarding](/telegram/message-forwarding)
*   [Message Filters](/telegram/message-filters)
*   [Greeting Message Notification](/telegram/greeting-message-notification)
*   [Other Settings](/telegram/other-settings)

## Suggested articles

*   [How to forward messages from a Telegram channel to Discord](/telegram/how-to-forward-messages-from-a-telegram-channel-to-discord)
*   [How to forward messages from a Telegram group to Discord](/telegram/how-to-forward-messages-from-a-telegram-group-to-discord)
