---
type: page
title: Order Workflows
seoTitle: Order Workflows
seoDescription: What are the Order workflows?
slug: order-workflows
order: 41
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# Order Workflows

# Order Workflows

****In this article:****

[What are the Order workflows?](#1-what-are-the-order-workflows)

[Possible Order workflows](#1-possible-order-workflows)

*   [1\. Notify customers about the orders and reward them via email](#2-notify-customers-about-the-orders-and-reward-them-via-email)
*   [2\. Get notified of the cancelled order](#2-get-notified-of-the-cancelled-order)
*   [3\. Add order tags when it is fulfilled and ask customers for a review](#2-add-order-tags-when-it-is-fulfilled-and-ask-customers-for-a-review)
*   [4\. Verify the high-risk order and get notified when it is placed](#2-verify-the-high-risk-order-and-get-notified-when-it-is-placed)
*   [5\. Create a real order from the draft and capture payment](#2-create-a-real-order-from-the-draft-and-capture-payment)

# ✔️ What are the Order workflows?

Order workflows are the flows that are launched by the Order triggers.

So, in this help guide, you'll find out more possible workflows related to the Orders (caused by the Order triggers) for different cases.

There are ****8**** Order triggers that can start a workflow to perform an action with the order:

*   Order created
*   Order deleted
*   Order cancelled
*   Order fulfilled
*   Order paid
*   Draft order created
*   Draft order deleted
*   Order transaction created

![](https://cdn.heymantle.com/docs/screenshots/f1158af1-feec-48eb-a0e1-ff549d55daae/triggers_110lx18.png)

Depending on the selected trigger you can create different workflows with different aims.

****It can be:****

*   customer notification about the new order,
*   marking the specific order by tags or adding metafields,
*   rewarding customers with gifts via email,
*   actions with the payment process,
*   fraud risk analysis,
*   or some other actions with the order.

Let's check some of them in more detail.

# ✔️ Possible Order workflows

## Notify customers about the orders and reward them via email

Let's start with the very first trigger action that can be run in your store - ****Order created****.

In this case, we're going to consider the situation when a shop owner wants to:

*   mark the order if its amount is more than $200;
*   send a "Thank You" email to a customer who has made an order with a gift card inside.

So, this workflow will look like this:

1.  First, select the ****"Order created"**** trigger.
2.  Next, we should add a condition ****"Amount"**** and set if it is greater or equal to the value "200"
3.  Also, we need to add an action → select ****"Add customer tags"**** and write **VIP**.
4.  Add one more action - ****"Send email"**** where we reward the customer with a gift card and, by this, build his loyalty.

![](https://cdn.heymantle.com/docs/screenshots/dc9a779d-b8b4-4ae8-b3c4-f6498729d76e/notify-customers-about-discoun_bd8m24.png)

With this trigger it is possible to filter customers by their loyalty. For this, we can verify how long are they in our store.

Let's create another workflow:

1.  Select the same trigger - ****Order created****
2.  Add the ****Lifetime duration**** condition → and set is equal to ****6 months****. This way we'll be able to track the customers who have already been for 6 months in our store since they were added → Next, we add customer tag - "Top customer"
3.  If the customer's lifetime duration is less but is equal to ****3 months**** → we add the "Medium customer" tag
4.  Do the same for the customers whose lifetime duration is ****1 month**** and add "Beginner customer"

![](https://cdn.heymantle.com/docs/screenshots/bcc65540-8b14-45ac-926f-61679a1e0871/lifetime-duration_t0qmb2.png)

## Get notified of the cancelled order

In this case, a store owner will be notified via email when the order is cancelled.

1.  When an order is ****cancelled****, we need to establish the reason of the cancellation. → After selecting the ****"Order cancelled"**** trigger, choose the ****"Cancel reason"**** condition.
2.  Select the ****is equal**** matcher and set the ****"inventory"**** value to verify if the order was cancelled because of the product lack in the store inventory.
3.  If the condition is met → set the ****"Create redirect URL"**** action. This way, you will redirect the customer to your another store page with the similar product so he can buy it instead of the initial one. There are two URLs that you should paste - the one is for the store page with the initial order and the second is for the new one.
4.  After we've created a new URL, we need to get notified about the cancelled order in our store. Add one more action below - ****"Send email"**** - insert your own email and jot down the message about the cancellation.

![](https://cdn.heymantle.com/docs/screenshots/86fb4abc-7aac-4035-bb70-92b055d596dd/cancel-reason-inventory_1v314p2.png)

5.  Next, we should set one more condition in the case if the item in this order can be restocked. Choose the ****"Restockable"**** condition → then, select the ****"is true"**** matcher.
6.  To end this workflow, let's set the final action - ****"Send email"**** to the customer to inform him about the restocking of this item. The workflow is ready!

![](https://cdn.heymantle.com/docs/screenshots/443455d4-0200-420a-a7d1-60bddea1d8e2/cancel-reason_1s9r0qu.png)

## Add order tags when it is fulfilled and ask customers for a review

This workflow will be useful when an order has already been fulfilled and you want to receive a feedback from the customer.

1.  So, start with the trigger - ****Order fulfilled****.
2.  Next, set a condition - if ****Fulfillments**** → select the ****Any of fulfillments match the following**** matcher → set the ****Status**** condition → that is equal to ****Success****

![](https://cdn.heymantle.com/docs/screenshots/e3629df9-6b7a-484d-af36-c4efcddbd987/fulfillment-status-is-success_13djgw6.png)

3.  Before we add the final action, we need to set a two-day delay → click the ****"Delay"**** button → select ****Days**** in the time interval type → and set "2".
4.  The final step for this workflow is the ****Send email**** action where we should indicate customer's email, and write the text in the message field.

![](https://cdn.heymantle.com/docs/screenshots/0044c53b-d7e9-4c8a-b46a-dd36c61c8340/order-fulfilled_dh50p2.png)

We save all the changes, give the workflow a title, and enable it.

## Verify the high-risk order and get notified when it is placed

Sometimes, it happens that there are orders that can be potentially high-risk which means fraudulent. That's why it is important to detect them as earlier as possible.

Therefore, in this case we are going to create the following workflow:

1.  We'll start with the ****"Order paid"**** trigger when a customer has already paid it.
2.  If this order has already been marked as high-risk, we need to prevent its fulfillment. For this, add the ****Risk level**** condition and set ****"high"****.
3.  Then, add an action - ****Cancel order****. In the list below this action check the ****"Restock items"**** box in order to restock the items that were purchased back into your store.

![](https://cdn.heymantle.com/docs/screenshots/30349c2f-1c56-46f1-b495-af09682bdaa1/high-level-risk_1nffxto.png)

In this workflow, we can also consider another ****case**** - when the order is paid but a store owner wants to get notified if it still isn't fulfilled in two days and mark this order as paid.

The steps for this case will be the following:

1.  Click "otherwise" and let's add another condition choose the ****Display fulfillment status**** → select the ****"Unfulfilled"**** option
2.  The final action should be executed after two days since the order was paid → so, set a delay ****in two days****
3.  Add the order tag ****"unfulfilled"**** and enable the workflow.

![](https://cdn.heymantle.com/docs/screenshots/baf0aef0-07dc-4a11-b815-58205bb08295/unfulfilled-tag-order_1ry87r7.png)

## Create a real order from the draft and capture payment

In this case, we are going to create a real order from the draft. A draft order can be created by the store owner himself in different situations (e.g., when the order was made outside his store, )

1.  This workflow starts with the ****Draft order created**** trigger
2.  Next, it comes to verify order's status → select the ****Status**** condition and set the appropriate value - for example, ****is equal to**** "open"

![](https://cdn.heymantle.com/docs/screenshots/ffe72153-e233-4111-8ad6-bd1d260f5093/draft-order-created_1938dns.png)

3.  Also, let's tag this draft order, and when it will be needed to create a real one from it, we will easily find it among others → Select ****Add draft order tags**** and write "Draft order - needs fulfillment".
4.  Set the ****Send email**** action in order to get notified of a new draft order.

![](https://cdn.heymantle.com/docs/screenshots/fe74006a-c716-4b6a-82c5-f8de99ebeb06/draft-order-status-opened_92703o.png)

# ✔️ Main advantage

As you can see, React Flow really facilitates your routine work and saves you a lot of time. With just a few clicks, you can set up automated workflows to efficiently handle key processes for multiple customers at once. This allows you to organize customers into groups using appropriate characteristics or tags, eliminating the need to focus on individual customers manually.

## Suggested articles

*   [Components of the workflow](/components-of-the-workflow)
*   [Most popular flows](/most-popular-flows)
*   [Customer Workflows](/customer-workflows)

Updated on: 25/03/2026