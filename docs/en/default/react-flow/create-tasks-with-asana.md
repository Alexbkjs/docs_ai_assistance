---
type: page
title: Create tasks with Asana
seoTitle: Create tasks with Asana
seoDescription: What is Asana?
slug: create-tasks-with-asana
order: 10
status: published
---


# Configure the Asana connector and create tasks

## What is Asana?

Asana is a work management service that allows teams to organize, track, and manage their work. Integrating with Asana lets you create tasks directly within React Flow.

## How to connect Asana to React Flow?

**1. Asana — Create account**

To connect Asana to React Flow, you need an Asana account. If you already have one, log in and skip this step. Otherwise, register at Asana.

Log in to your account and create your project. Note the project ID — you will need it in React Flow.

**2. React Flow — Create Asana connector**

Open the React Flow app → **Connectors tab** → click on **Asana connector**.

Step 1. (optional) Enter the name and description of the connector.

Step 2. Click the link in the description and copy your **Auth Token** → enter it in the appropriate field in React Flow.

![Configure Asana connector](https://cdn.heymantle.com/docs/screenshots/940cb93c-83ce-439b-957a-ae2adddaeaf8/asasna-connector-info_9804e7.png)

Make sure to copy the provided access token — you won't see it again.

Step 3. Click **Test** to check whether the connector works correctly. Enter your project ID → click **Test**.

To find your project ID, go to your Asana profile, open your project, and copy the ID from the address bar as shown in the screenshot below.

![Copy your project id](https://cdn.heymantle.com/docs/screenshots/afcc6c6b-32a3-4d84-9f61-f18d9c474afd/asana-project-id_ngl7lo.png)

Step 4. **Save** the configuration.

## Create Asana task action

The Asana task action lets you automatically send tasks to Asana.

Example: You want to create a task every time an order is created.

1.  Open the React Flow app and click **Create new**.
2.  Select the **Order created** trigger.
3.  Click **Add action** and select **Create Asana task** in the right-side menu.
4.  Click **Select connection** and select your Asana connector.
5.  Enter the task name and description.

![](https://cdn.heymantle.com/docs/screenshots/7c88b0ad-e530-4493-8bcd-00b0ee9e0f23/select-asana-task_1e0ihug.png)

6.  **Save** the configuration.

## Useful link

*   Learn more about all [Available React Flow connectors](/react-flow/react-flow-connectors).

## Suggested articles:

*   [React Flow connectors](/react-flow/react-flow-connectors)
*   [Send email with SMTP connector](/react-flow/send-email-with-smtp-connector)
*   [Send SMS and WhatsApp messages with Twilio](/react-flow/send-sms-and-whatsapp-messages-with-twilio)
