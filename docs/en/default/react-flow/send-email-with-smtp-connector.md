---
type: page
title: Send email with SMTP connector
seoTitle: Send email with SMTP connector
seoDescription: What is SMTP?
slug: send-email-with-smtp-connector
order: 3
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# Send email with SMTP connector

# Configure SMTP connector

In this article:

*   [What is SMTP?](#1-what-is-smtp)
*   [How to activate SMTP connector?](#1-how-to-activate-smtp-connector)
*   [Send email action](#1-send-email-action)
*   [Available connectors](#1-available-connectors)

# ✔️ What is SMTP and SMTP connector?

SMTP is a simple communication protocol used to send emails from a sender's server to a recipient's server. The SMTP connector allows you to connect external email hosting provider and use your personal authorized business email as the sender for all Send email actions.

# ✔️ How to activate SMTP connector?

Enter the React Flow app > Connectors tab > click on SMPT connector.

![Select SMTP connector](https://cdn.heymantle.com/docs/screenshots/e22bb915-2102-4015-800d-0641e2ed36df/select-smtp_1fbf1lo.png)

1.  (optional) Enter the name and description of the connector.
2.  Select a provider from the drop-down list below.
3.  Enter your user name, password and email. We have prepared [an article](/google-email-hosting-provider) in which you can find information on where to get this data.

If you did not find the desired provider, you can set up a custom one. To configure it, contact your provider's support and specify the required data. You can also contact our support, we will answer you as soon as possible.

4.  In the upper right corner click on the Test button - it is designed to check the correct information. Please use it to ensure that you have entered the correct information.

![Enter required data](https://cdn.heymantle.com/docs/screenshots/91d98a31-f6ee-48df-bf41-b22917c7b5a7/smtp-connection-details_15az39k.png)

5.  ****Save**** configuration.

# ✔️ Send email action

Send email action allows you automatically send email letters to your customer.

Example: a customer has created an order but hasn’t paid for it. You want to send him a payment reminder email.

1.  Such a workflow is already in the [Templates](/react-flow-templates) and you can quickly set it up. Click on ****Templates****.
2.  Find and click ****Sending a reminder of unpaid orders to users****.

![Select a template](https://cdn.heymantle.com/docs/screenshots/1dd076b3-6cdb-44b9-a4a7-be04bd8b6f7f/select-sending-a-reminder-temp_ed8fr.png)

3.  Customize the template. For example, the letter is scheduled to be sent in 2 days. You can change this number.
4.  Сlick on ****Send email****.
5.  In the Connection field click ****Change**** and choose your provider.

![](https://cdn.heymantle.com/docs/screenshots/edbce41e-5664-4c7f-be0d-8f3412e4b0f9/set-connector_cg68ep.png)

6.  ****Save**** your workflow in the upper right corner.
7.  ****Turn on workflow**** in the upper right corner.

Now the client receives a letter with the address of your store.

# ✔️ Useful link

*   Learn more about all [Available React Flow connectors](/react-flow-connectors).

Updated on: 27/02/2026