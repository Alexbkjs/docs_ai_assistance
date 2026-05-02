---
type: page
title: Send email with SMTP connector
seoTitle: Send email with SMTP connector
seoDescription: What is SMTP?
slug: send-email-with-smtp-connector
order: 3
status: published
---


# Configure SMTP connector

## What is SMTP and the SMTP connector?

SMTP is a communication protocol used to send emails from a sender's server to a recipient's server. The SMTP connector lets you connect an external email hosting provider and use your authorized business email as the sender for all Send email actions.

## How to activate the SMTP connector?

Open the React Flow app → Connectors tab → click on the SMTP connector.

![Select SMTP connector](https://cdn.heymantle.com/docs/screenshots/e22bb915-2102-4015-800d-0641e2ed36df/select-smtp_1fbf1lo.png)

1.  (optional) Enter the name and description of the connector.
2.  Select a provider from the drop-down list.
3.  Enter your username, password, and email. We have prepared [an article](/react-flow/google-email-hosting-provider) explaining where to find this information.

If your provider is not listed, you can configure a custom one. Contact your provider's support for the required settings. You can also contact our support team and we will help you as soon as possible.

4.  Click the **Test** button in the upper right corner to verify that you have entered the correct information.

![Enter required data](https://cdn.heymantle.com/docs/screenshots/91d98a31-f6ee-48df-bf41-b22917c7b5a7/smtp-connection-details_15az39k.png)

5.  **Save** the configuration.

## Send email action

The Send email action lets you automatically send emails to your customers.

Example: a customer has created an order but has not paid for it, and you want to send a payment reminder.

1.  This workflow is already available in [Templates](/react-flow/react-flow-templates). Click **Templates**.
2.  Find and click **Sending a reminder of unpaid orders to users**.

![Select a template](https://cdn.heymantle.com/docs/screenshots/1dd076b3-6cdb-44b9-a4a7-be04bd8b6f7f/select-sending-a-reminder-temp_ed8fr.png)

3.  Customize the template. For example, the email is scheduled to be sent after 2 days — you can change this value.
4.  Click on **Send email**.
5.  In the Connection field, click **Change** and choose your provider.

![](https://cdn.heymantle.com/docs/screenshots/edbce41e-5664-4c7f-be0d-8f3412e4b0f9/set-connector_cg68ep.png)

6.  **Save** your workflow using the button in the upper right corner.
7.  **Turn on workflow** using the button in the upper right corner.

Your customers will now receive emails from your store's address.

## Useful link

*   Learn more about all [Available React Flow connectors](/react-flow/react-flow-connectors).
