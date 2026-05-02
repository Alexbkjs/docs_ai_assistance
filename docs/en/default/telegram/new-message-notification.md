---
type: page
title: New Message Notification
seoTitle: New Message Notification
seoDescription: This option allows you to customize messages for users, groups, or channels. You can personalize them to create a more welcoming and pleasant experience for your audience.
slug: new-message-notification
order: 8
status: published
---

Articles on: [Telegram](/en/category/telegram-1urqa6t/)

# New Message Notification

  

# Manage New Message Notification

  

This option allows you to customize messages for users, groups, or channels. You can personalize them to create a more welcoming and pleasant experience for your audience.

  

To customize the message, follow these steps:

  

1.  Use the `/list` command to bring up a modal window with settings.
2.  Click on ****Settings**** -> Choose the settings -> ****New Message Notification****.
3.  Select which message you want to edit and click ****Edit notification****.

  

![](https://cdn.heymantle.com/docs/screenshots/e25c04e9-075d-4a3e-9952-8bfe0fcb756e/edit-message-notification_tuc7h7.png)

  

In the appeared window you can enter the message that you want to display and click Submit.

  

You can use the following variables to customize your welcome message:

  

*   `{{fullName}}`: Displays the user's full name (e.g., ****John Smith****).

Note: This does not create a link to the user's Telegram chat.

*   `{{userName}}`: Displays the user's username as a clickable link (e.g., ****@john\_smith****).

Note: Not all users have a username, but every user will have a full name.

*   `{{name}}`: Automatically selects either the {{fullName}} or {{userName}}, depending on availability. If the username exists, it will be used; otherwise, the full name will be displayed.

  

![](https://cdn.heymantle.com/docs/screenshots/514917eb-4181-495a-a63d-33511fa20798/new-message_t98da2.png)

  

Note: Telegram allows you to create public and private groups/channels. Public groups will include links if the variables {{userName}} or {{name}} are used. If groups or channels are private, only the group name will be displayed, without a link, regardless of the assigned variable.

  

In the Settings section, you can also customize:

  

*   [Message Forwarding](/message-forwarding)
*   [Message Filters](/message-filters)
*   [Greeting Message Notification](/greeting-message-notification)
*   [Other Settings](/other-settings)

  

## Suggested articles

  

*   [How to forward messages from a Telegram channel to Discord](/how-to-forward-messages-from-a-telegram-channel-to-discord)
*   [How to forward messages from a Telegram group to Discord](/how-to-forward-messages-from-a-telegram-group-to-discord)

  

Updated on: 21/05/2025