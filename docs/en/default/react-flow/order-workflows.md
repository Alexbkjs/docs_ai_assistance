---
type: page
title: Order Workflows
seoTitle: Order Workflows
seoDescription: What are the Order workflows?
slug: order-workflows
order: 41
status: published
---


# Order Workflows

## What are the Order workflows?

Order workflows are flows triggered by Order triggers.

In this guide, you'll find workflow examples related to Orders — covering various use cases.

There are **8** Order triggers that can start a workflow:

*   Order created
*   Order deleted
*   Order cancelled
*   Order fulfilled
*   Order paid
*   Draft order created
*   Draft order deleted
*   Order transaction created

![](https://cdn.heymantle.com/docs/screenshots/f1158af1-feec-48eb-a0e1-ff549d55daae/triggers_110lx18.png)

Depending on the selected trigger, you can create different workflows for different goals.

**Examples include:**

*   customer notification about a new order,
*   marking specific orders with tags or adding metafields,
*   rewarding customers with gifts via email,
*   actions related to the payment process,
*   fraud risk analysis,
*   or other order-related actions.

Let's explore some of them in detail.

## Possible Order workflows

### Notify customers about their orders and reward them via email

Let's start with the first trigger — **Order created**.

In this example, the store owner wants to:

*   tag the order if its amount is more than $200;
*   send a "Thank You" email to the customer with a gift card inside.

This workflow looks like this:

1.  Select the **"Order created"** trigger.
2.  Add an **"Amount"** condition and set it to greater than or equal to "200".
3.  Add an action → select **"Add customer tags"** and write **VIP**.
4.  Add one more action — **"Send email"** — to reward the customer with a gift card and build loyalty.

![](https://cdn.heymantle.com/docs/screenshots/dc9a779d-b8b4-4ae8-b3c4-f6498729d76e/notify-customers-about-discoun_bd8m24.png)

You can also filter customers by loyalty — for example, how long they've been in your store.

Create another workflow:

1.  Select the same trigger — **Order created**.
2.  Add the **Lifetime duration** condition → set it equal to **6 months** to track customers who have been in your store for 6 months → add the customer tag "Top customer".
3.  If the customer's lifetime duration is equal to or less than **3 months** → add the "Medium customer" tag.
4.  Do the same for customers with a **1-month** lifetime and add the "Beginner customer" tag.

![](https://cdn.heymantle.com/docs/screenshots/bcc65540-8b14-45ac-926f-61679a1e0871/lifetime-duration_t0qmb2.png)

### Get notified of a cancelled order

In this example, the store owner receives an email notification when an order is cancelled.

1.  After selecting the **"Order cancelled"** trigger, choose the **"Cancel reason"** condition to determine why the order was cancelled.
2.  Select the **is equal** matcher and set the value **"inventory"** to check whether the order was cancelled due to insufficient stock.
3.  If the condition is met → set the **"Create redirect URL"** action to redirect the customer to another store page with a similar product. Provide two URLs — one for the original product page and one for the replacement.
4.  Add a **"Send email"** action to notify yourself about the cancelled order.

![](https://cdn.heymantle.com/docs/screenshots/86fb4abc-7aac-4035-bb70-92b055d596dd/cancel-reason-inventory_1v314p2.png)

5.  Add one more condition to check whether the item in this order can be restocked. Choose the **"Restockable"** condition → select the **"is true"** matcher.
6.  Set the final action — **"Send email"** — to notify the customer about the restocking of this item. The workflow is ready.

![](https://cdn.heymantle.com/docs/screenshots/443455d4-0200-420a-a7d1-60bddea1d8e2/cancel-reason_1s9r0qu.png)

### Add order tags when fulfilled and ask customers for a review

This workflow is useful when an order has been fulfilled and you want to request customer feedback.

1.  Start with the **Order fulfilled** trigger.
2.  Set a condition — if **Fulfillments** → select **Any of fulfillments match the following** → set the **Status** condition → equal to **Success**.

![](https://cdn.heymantle.com/docs/screenshots/e3629df9-6b7a-484d-af36-c4efcddbd987/fulfillment-status-is-success_13djgw6.png)

3.  Before adding the final action, set a two-day delay → click **"Delay"** → select **Days** as the time interval type → set "2".
4.  The final step is the **Send email** action — enter the customer's email address and write the message text.

![](https://cdn.heymantle.com/docs/screenshots/0044c53b-d7e9-4c8a-b46a-dd36c61c8340/order-fulfilled_dh50p2.png)

Save all changes, give the workflow a title, and enable it.

### Verify a high-risk order and get notified when it is placed

Some orders may be potentially fraudulent, so it's important to detect them as early as possible.

1.  Start with the **"Order paid"** trigger.
2.  Add the **Risk level** condition and set it to **"high"** to flag already-paid high-risk orders.
3.  Add the **Cancel order** action. Check the **"Restock items"** box to return the purchased items to your store inventory.

![](https://cdn.heymantle.com/docs/screenshots/30349c2f-1c56-46f1-b495-af09682bdaa1/high-level-risk_1nffxto.png)

You can also handle another case — when the order is paid but remains unfulfilled after two days:

1.  Click "otherwise" and add the **Display fulfillment status** condition → select the **"Unfulfilled"** option.
2.  Set a delay of **two days**.
3.  Add the order tag **"unfulfilled"** and enable the workflow.

![](https://cdn.heymantle.com/docs/screenshots/baf0aef0-07dc-4a11-b815-58205bb08295/unfulfilled-tag-order_1ry87r7.png)

### Create a real order from a draft and capture payment

In this example, a real order is created from a draft. A draft order can be created by the store owner in various situations (e.g., when an order was placed outside the store).

1.  Start with the **Draft order created** trigger.
2.  Verify the order's status → select the **Status** condition and set the appropriate value — for example, **is equal to** "open".

![](https://cdn.heymantle.com/docs/screenshots/ffe72153-e233-4111-8ad6-bd1d260f5093/draft-order-created_1938dns.png)

3.  Tag this draft order so it's easy to find later → select **Add draft order tags** and write "Draft order - needs fulfillment".
4.  Set the **Send email** action to be notified of the new draft order.

![](https://cdn.heymantle.com/docs/screenshots/fe74006a-c716-4b6a-82c5-f8de99ebeb06/draft-order-status-opened_92703o.png)

## Main advantage

As you can see, React Flow simplifies your routine work and saves significant time. With just a few clicks, you can set up automated workflows to efficiently handle key processes for multiple customers at once — organizing them into groups using tags, without any manual effort.

## Suggested articles

*   [Components of the workflow](/react-flow/components-of-the-workflow)
*   [Most popular flows](/react-flow/most-popular-flows)
*   [Customer Workflows](/react-flow/customer-workflows)
