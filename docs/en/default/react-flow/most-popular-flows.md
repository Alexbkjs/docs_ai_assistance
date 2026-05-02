---
type: page
title: Most Popular Flows
seoTitle: Most Popular Flows
seoDescription: Hide out of stock products or Back in stock available products
slug: most-popular-flows
order: 9
status: published
---


# Popular Flows

In this article, you'll find the most popular workflows. You can use any of these examples to automate your Shopify store with React Flow. The app's functionality is extensive, and you can adapt flows to almost any situation — related to a product, order, customer, and more. If you can't find the right workflow for what you want to implement, write to our support team and we'll try to help. Some of these flows are also available as templates.

## Hide out of stock products or bring back in-stock products

This flow helps store owners automatically hide or re-publish products based on availability, so you don't need to track every item manually.

Choose **Inventory quantity changed** as the trigger.

Set the condition: **Product / Total inventory** less than or equal to 0.

Add the action **Hide product** to make the product unavailable in the online store.

![](https://cdn.heymantle.com/docs/screenshots/006f5e60-ba10-45bd-8eec-50b3fc36b006/hide-product_dugp9t.png)

You can set up the same flow to reactivate products. Change the condition to **greater than or equal to** and add the action **Activate product**.

## Product quantity alert

To receive low-stock alerts and restocking reminders automatically:

Select the **Inventory quantity change** trigger.

Set the condition: **Product variant / Inventory quantity** → set "less than or equal to" zero.

Then choose the **Send email** action.

![](https://cdn.heymantle.com/docs/screenshots/e6e9c5de-44fc-44e6-852c-5abf309a9942/inventory-quantity-changed_mgab3b.png)

## Cancel high-risk orders

You can protect your Shopify store from fraud by automatically cancelling orders from suspicious sources.

Choose **Order created** as the trigger.

Set the condition: **Order / Risk level** is equal to "High".

Add the action **Cancel order** or choose another action from the list.

In the reason field, select **Fraudulent order**. You can also send a notification explaining why the order was cancelled.

![](https://cdn.heymantle.com/docs/screenshots/f3912920-4f29-4798-a63f-b64e6717231d/cancel-order_i042sx.png)

## Tag the order by purchased products

With this workflow, you can tag fulfilled orders to identify which items are purchased most often. You can set up a flow to tag all products in a collection or products that contain certain words.

Select the **Order created** trigger.

Select **Order / Line items** as the condition and set the words the tag should include.

Add an "Action" and set the tag.

![](https://cdn.heymantle.com/docs/screenshots/2289cbe4-0f55-4331-ab05-82aaacfb1beb/add-order-tag_gcjith.png)

## Send a reminder for unpaid orders

A convenient flow to remind customers about an unpaid order. If a buyer created an order but forgot to pay, you can send them a reminder.

Choose **Order created** as the trigger.

Set the condition: **Order / Display financial status** → select "is any of" and choose the appropriate statuses, such as "Partially paid", "Pending", etc.

Add the **Send email** action.

![](https://cdn.heymantle.com/docs/screenshots/944381fd-c8f5-4d0e-9d90-b35f3c79884c/unpaid-order_li0jcj.png)

You have two options for sending the email. One option is to send via an **SMTP connector**. Learn more about this in [this article](/react-flow/react-flow-connectors).

## New products notification

Another popular flow for Shopify store owners is **New products notification**. When a new product or collection appears in the store, you can notify customers about it.

Select the **Order created** trigger. Optionally, set a delay or add conditions, then add the action **Send new product notification**. Don't forget to write a subject line and message for your customers.

![](https://cdn.heymantle.com/docs/screenshots/f5f56ade-1b2b-4408-8e64-5c7d48c5b8a3/new-product-notification_93wr3v.png)

## Thank you message

Staying in touch shows customers they matter to you. Send thank-you emails after each fulfilled, paid order or to welcome new customers.

Select the **Order created** trigger.

Select the **Order / Customer accepts marketing** condition and set it to "is true".

Add the **Send email** action.

![](https://cdn.heymantle.com/docs/screenshots/1a40c645-4db7-432a-8d50-2263632b32c7/thank-you-message_ncdecu.png)

## Low stock items report

Receive a daily low stock items report to your store's email address. These daily reports help you monitor inventory levels and prevent stockouts.

Trigger: **Time of day**.

Action: **Send low inventory products report** — set the exact time the report will be sent.

![](https://cdn.heymantle.com/docs/screenshots/d82d32eb-a5e4-4b4c-9802-11dc1a8a9a82/time-of-day_febbo8.png)

## Supplier notification

If you work with vendors and need to send them reports on products sold, set this up once and the reports will be sent automatically.

Choose **Order line item created** as the trigger.

Then set **Line item / Vendor = Vendor for mailing**.

Add the **Send email** action.

![](https://cdn.heymantle.com/docs/screenshots/17fb87ad-4a30-4cf7-a468-d85cb45c7d6e/order-line-item-created_dqmfff.png)

## Marketing tags

The Marketing tags workflow lets you identify customers who have given permission to receive store emails with news, offers, and promotions. This helps you build a marketing strategy based on email newsletters and increase your revenue.

Use the **Customer created** trigger.

Set the **Customer / Accepts marketing true** condition.

Then assign a **Tag** to this group of customers.

![](https://cdn.heymantle.com/docs/screenshots/d67e9533-0c61-40b1-aa28-1d4d6b3c19b7/marketing-tags_1sy7dzn.png)

## Useful links

*   [Order Workflows](https://help.devit.software/en/article/order-workflows-1hqqsbz/#2-verify-the-high-risk-order-and-get-notified-when-it-is-placed)
*   [Product Workflows](/react-flow/product-workflows)
*   [React Flow Triggers and Actions](/react-flow/react-flow-triggers-actions)
