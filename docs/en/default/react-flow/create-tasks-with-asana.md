---
type: page
title: Create tasks with Asana
seoTitle: Create tasks with Asana
seoDescription: What is Asana?
slug: create-tasks-with-asana
order: 10
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# Create tasks with Asana

# Configure the Asana connector and create tasks

****In this article:****

*   [What is Asana?](#1-what-is-asana)
*   [How to connect Asana to React Flow?](#1-how-to-connect-asana-to-react-flow)
*   [Create Asana task action](#1-create-asana-task-action)

# ✔️ What is Asana?

Asana is a work management service that allows teams to organize, track, and manage their work. Integration with Asana allows you to create tasks within the React Flow.

# ✔️ How to connect Asana to React Flow?

****1\. Asana - Create account****

To connect Asana to React Flow, you need an account in the Asana service. If you have an account, log in and skip this step. If you don’t, register there.

Log in to your account and create your project. Check the project ID. You will need it in React Flow.

****2\. React Flow - Create Asana connector****

Open the React Flow app > ****Connectors tab**** > click on ****Asana connector****.

Step 1. (optional) Enter the name and description of the connector.

Step 2. Click on the link in the description and copy ****Auth Token**** > enter it in the appropriate field in React Flow.

![Configure Asana connector](https://cdn.heymantle.com/docs/screenshots/940cb93c-83ce-439b-957a-ae2adddaeaf8/asasna-connector-info_9804e7.png)

Make sure to copy provided access token. You won't see it again.

Step 3. Click on ****Test****. It is designed to check if the connector works correctly. Enter your project id > click on ****Test****.

To get your project id, go to Asana profile, open your project and copy id from the address bar as it shown on screenshot below.

![Copy your project id](https://cdn.heymantle.com/docs/screenshots/afcc6c6b-32a3-4d84-9f61-f18d9c474afd/asana-project-id_ngl7lo.png)

Step 4. ****Save**** configuration.

# ✔️ Create Asana task action

The Asana task action allows you automatically send tasks to Asana.

Example: You want to create a task every time when the order is created.

1.  Open the React Flow app and click on ****Create new****.
2.  Select trigger ****Order created****.
3.  Click on ****Add action**** and in the right side menu select ****Create Asana task****.
4.  Click on ****Select connection**** and select Asana connector.
5.  Enter task name and description.

![](https://cdn.heymantle.com/docs/screenshots/7c88b0ad-e530-4493-8bcd-00b0ee9e0f23/select-asana-task_1e0ihug.png)

6.  ****Save**** configuration.

# ✔️ Useful link

*   Learn more about all [Available React Flow connectors](/react-flow-connectors).

## Suggested articles:

*   [React Flow connectors](/react-flow-connectors)
*   [Send email with SMTP connector](/send-email-with-smtp-connector)
*   [Send SMS and WhatsApp messages with Twilio](/send-sms-and-whatsapp-messages-with-twilio)

Updated on: 02/03/2026