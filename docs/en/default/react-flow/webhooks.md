---
type: page
title: Webhooks
seoTitle: Webhooks
seoDescription: What are webhooks?
slug: webhooks
order: 17
status: published
---


# Webhooks

## What are webhooks?

**Webhooks** are automated notifications that send real-time data from third-party services to your store via a URL you provide. Instead of constantly polling for updates, a webhook instantly notifies another service by sending data to that URL. The data is delivered in JSON or XML format.

Webhooks make it easy to extend the app's functionality by connecting it to additional third-party services or custom systems.

## How to connect a webhook to React Flow?

1.  Go to the React Flow admin and create a new workflow.
2.  In the right-side menu, select the **Webhook event** trigger.

![](https://cdn.heymantle.com/docs/screenshots/bd39eff5-bc4b-469c-9b67-037e76890c01/select-webhook-event_1keca8y.png)

3.  Click **Select webhook** → Create new webhook.
4.  In the window that opens, configure the available settings:

*   Go to the **Path** section and enter a path name. The app will generate a unique URL that you can use in subsequent steps.
*   You can also choose the HTTP method and authentication options.

5.  Click **Create**.

![](https://cdn.heymantle.com/docs/screenshots/bb6f0a8d-7546-4544-8e47-740bb491c621/create-webhook_1lzldg8.png)

You have now generated a unique URL that you can paste into the third-party service to connect it with React Flow.

After that, you can continue building your workflow by clicking the **+** icon in the trigger block.

## Need help?

If this feels technical, our support team can guide you through the process or set up the webhook for you. Send us a message: [support@devit.software](mailto:support@devit.software)
