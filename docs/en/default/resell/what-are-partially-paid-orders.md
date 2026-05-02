---
type: page
title: What are partially paid orders?
seoTitle: What are partially paid orders?
seoDescription: What is the reason for partially paid orders?
slug: what-are-partially-paid-orders
order: 15
status: published
---


# Partially paid orders

## What causes partially paid orders?

Sometimes a customer accepts a post-purchase upsell offer but receives a payment declined message.

There are **2 reasons** that lead to partially paid orders:

*   Insufficient funds on the customer's card.
*   The payment processor denies the transaction.

## How does it happen?

When payment for the post-purchase upsell offer fails, Shopify still adds the upsell product to the primary order. This creates a situation where the primary order is paid but the upsell product is not. The order becomes stuck and cannot be completed.

Important: ReSell does **NOT** control the payment process. The app does not affect monetary transactions between the customer and the seller in any way.

## What does a customer see for partially paid orders?

When a customer accepts a post-purchase upsell offer and the payment fails, they are redirected to the order confirmation page. There, they are notified that the product has been added to the order but payment is still required. The message also prompts them to pay the outstanding amount.

If the additional item remains unpaid, Shopify sends an invoice email after 2 hours.

Shopify does not send an invoice email if the additional item has already been paid or has been removed from the order.

## How to identify partially paid orders

To track partially paid orders, check their status in your **Shopify admin**. Look for orders with the payment status **Partially paid**.

![](https://cdn.heymantle.com/docs/screenshots/6028d18f-a21e-4a81-bb9d-43e22715bd50/partially-paid-orders_1ouc857.png)

In the order timeline, you will find detailed information about the order and any payment processing errors.

## Resolving partially paid orders

To resolve partially paid orders, try the following options:

1.  **Collect payment for the order.** This is the more profitable and preferred option. The customer already accepted the offer, meaning they are interested in the product and are likely to pay. If the additional product remains unpaid after two hours, Shopify will send an invoice to remind them. Note that this does not guarantee payment — see the next option for handling orders with unpaid upsell items.

2.  **Remove the unpaid item from the order.** If the customer does not pay for the upsell product, you need to remove it so the main order can be completed. The product must be either paid for or removed from the order.

ReSell includes a built-in option to remove unpaid items automatically.

To enable this option:

*   Go to **Settings** in the left-side menu.
*   Enable **Automatically remove unpaid 1-click upsell products from orders**.
*   (Optional) Enable the option to send an order update email to the customer when products are removed.
*   **Set the time limit** after which the product should be removed if the order remains unpaid (for example, 60 minutes).
*   Save the settings.

![](https://cdn.heymantle.com/docs/screenshots/bd60137d-36df-470f-b6c3-d97fdd5084ad/partially-paid-settings_1ea4yj0.png)

If a customer accepts an additional upsell product but has insufficient funds to complete the payment, the product will be automatically removed after the set time, and the order status will be updated to "Paid."

## Next step

Learn more about how to [customize your offers](/resell/can-i-customize-my-offers) and check examples of popular offers to [get maximum benefits using ReSell](/resell/get-maximum-benefits-using-resell).
