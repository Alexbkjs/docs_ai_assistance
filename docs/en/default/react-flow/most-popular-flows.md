---
type: page
title: Most Popular Flows
seoTitle: Most Popular Flows
seoDescription: Hide out of stock products or Back in stock available products
slug: most-popular-flows
order: 9
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# Most Popular Flows

# Popular Flow

****In this article:****

*   [Hide out of stock products or Back in stock available products](#1-hide-out-of-stock-products-or-back-in-stock-available-products)
*   [Product quantity alert](#1-product-quantity-alert)
*   [Cancel high risk order](#1-cancel-high-risk-order)
*   [Tag the order by purchased products](#1-tag-the-order-by-purchased-products)
*   [Sending a reminder of unpaid orders to users](#1-sending-a-reminder-of-unpaid-orders-to-users)
*   [New products notification](#1-new-products-notification)
*   [Thank you message](#1-thank-you-message)
*   [Low stock items report](#1-low-stock-items-report)
*   [Supplier notification](#1-supplier-notification)
*   [Marketing tags](#1-marketing-tags)

In this article you will find the most popular workflows. You can use one of the scripts to automate your Shopify store with React Flow App. The functionality of the application is huge and you can adjust the flow for almost any situation. A workflow can be related to a product, order, customer, etc. If you can not find the right workflow for the situation you want to implement and use in your store - you can write to our support and we will try to help you. You can find some of these flows in templates, use them to customize the processes in your store.

# ✔️ Hide out of stock products or Back in stock available products

This flow can help store owners automatically hide or repost products based on availability. You don't need to track every item and do it manually.

For this flow choose ****Inventory quantity changed**** as a trigger.

Condition is ****Product / Total inventory**** less than or equal to 0.

Now add action ****Hide product**** - make the product that triggered this workflow unavailable on the online store.

![](https://cdn.heymantle.com/docs/screenshots/006f5e60-ba10-45bd-8eec-50b3fc36b006/hide-product_dugp9t.png)

You can set up the same flow to activate the product in the store. Change the conditions to ****greater than or equal to**** and add action ****Activate product**** .

# ✔️ Product quantity alert

If you'd like to receive low-stock alerts and reminders to refill, you can also set this up automatically.

To do this, select a trigger ****Inventory quantity change****.

And select condition when ****Product variant / Inventory quantity**** -> set the condition “less than or equal to” and enter zero.

Then choose ****Send email**** action.

![](https://cdn.heymantle.com/docs/screenshots/e6e9c5de-44fc-44e6-852c-5abf309a9942/inventory-quantity-changed_mgab3b.png)

# ✔️Cancel high risk order

You can also protect the store on Shopify from fraudsters with the help of the React Flow application functionality. For instance, you can automatically cancel orders from dangerous emails.

Choose ****Order created**** as a trigger.

Condition is ****Order / Risk level**** is equal “High”.

And add action ****Cancel order**** or choose any other action from the list.

In the reason field select ****Fraudulent order**** . You can also send notification explaining why the order was canceled.

![](https://cdn.heymantle.com/docs/screenshots/f3912920-4f29-4798-a63f-b64e6717231d/cancel-order_i042sx.png)

# ✔️Tag the order by purchased products

With this workflow, you can add tags to fulfield orders to see which items are purchased more often than others. You can set up an automatic flow that will tag, for example, all products in a collection or products that contain certain words.

Select ****Order created**** trigger.

Select ****Order / Line items**** as a condition and set the words that the tag should include.

Add “Action” and set the tag.

![](https://cdn.heymantle.com/docs/screenshots/2289cbe4-0f55-4331-ab05-82aaacfb1beb/add-order-tag_gcjith.png)

# ✔️Sending a reminder of unpaid orders to users

A convenient flow to remind your customers about an unpaid order. Let's imagine that the buyer created an order, but for some reason did not have time or forgot to pay. You can send him or her a reminder letter.

Choose ****Order created**** as a trigger.

Condition is ****Order / Display financial status**** -> select ‘is any of’ and select the appropriate parameters like “Partially paid”, “Pending”, etc.

And add action ****Send email****.

![](https://cdn.heymantle.com/docs/screenshots/944381fd-c8f5-4d0e-9d90-b35f3c79884c/unpaid-order_li0jcj.png)

Let us remind that here you have two options to send a letter. One of them is Send an email to an email address via ****SMPT connector****. In [this article](/react-flow-connectors) we told you about it in detail.

# ✔️ New products notification

Another popular flow used by Shopify shop owners is ****New products notification****. If a new product or collection has appeared in the store, you can notify clients about it.

Select trigger ****Order created****. If you want, you can set the delay or add conditions, and then add action ****Send new product notification****. Don't forget to write subject of the letter and message for your customers.

![](https://cdn.heymantle.com/docs/screenshots/f5f56ade-1b2b-4408-8e64-5c7d48c5b8a3/new-product-notification_93wr3v.png)

# ✔️ Thank you message

It is important for every customer that the store keeps in touch with him. To show that each customer is important to you, you can send thank-you letters after each fulfield and paid order or to welcome new customers, for instance.

Select ****Order created**** trigger.

Select \*\*Order / Customer accepts marketing” condition and select ‘is true’.

And ****Send email**** action.

![](https://cdn.heymantle.com/docs/screenshots/1a40c645-4db7-432a-8d50-2263632b32c7/thank-you-message_ncdecu.png)

# ✔️ Low stock items report

With the help of the application, you can receive a daily Low stock items report to the store owner's email. These daily reports will help to control the amount of goods in the store and avoid the situation when the goods are not available.

Trigger is ****Time of day****.

Action is ****Send low inventory products report**** and set the exact time the report will be sent.

![](https://cdn.heymantle.com/docs/screenshots/d82d32eb-a5e4-4b4c-9802-11dc1a8a9a82/time-of-day_febbo8.png)

# ✔️ Supplier notification

Cooperating with some vendors, you are obliged to send them reports with the number of products sold. After setting up the workflow once, these reports will be sent automatically without your involvement.

Choose ****Order line item created**** as a trigger.

Than ****Line item / Vendor = Vendor for mailing****.

And ****Send email**** action.

![](https://cdn.heymantle.com/docs/screenshots/17fb87ad-4a30-4cf7-a468-d85cb45c7d6e/order-line-item-created_dqmfff.png)

# ✔️Marketing tags

And last but not least Marketing tags workflow. You can use this flow to single out customers, who have given permission to receive emails from the store with news, offers, promotions, etc. With the help of this workflow, you can build a marketing strategy based on email newsletters and increase your profits.

Use ****Customer created**** trigger.

****Customer / Accepts marketing true**** condition.

And give ****Tag**** for these group of clients.

![](https://cdn.heymantle.com/docs/screenshots/d67e9533-0c61-40b1-aa28-1d4d6b3c19b7/marketing-tags_1sy7dzn.png)

## Useful links

*   [Order Workflows](https://help.devit.software/en/article/order-workflows-1hqqsbz/#2-verify-the-high-risk-order-and-get-notified-when-it-is-placed)
*   [Product Workflows](/product-workflows)
*   [React Flow Triggers and Actions](/react-flow-triggers-actions)

Updated on: 27/02/2026