---
type: page
title: Customer Workflows
seoTitle: Customer Workflows
seoDescription: What are the Customer workflows?
slug: customer-workflows
order: 25
status: published
---


# Customer Workflows

## What are the Customer workflows?

Building trust with customers is a top priority for any business owner, as it is the foundation for future growth. Throughout the day, it's essential to maintain effective communication and address various issues such as shipping, refunds, email correspondence, and risk verification.

For this category, the following triggers can run workflows:

*   Customer created
*   Customer deleted
*   Customer account enabled
*   Customer account disabled

In this guide, we'll look at some workflow examples for the **"Customers"** category.

## Send a thank-you email to a new customer and build loyalty

1.  Start with the **Customer created** trigger.
2.  Verify whether this customer agreed to receive marketing materials → select the **Accepts marketing** condition and set "is true".
3.  Once a new customer has joined your store, send them an email with a 3-day gift coupon as a welcome offer → set a **Delay** of 1 day before the **Send email** action.
4.  To quickly identify new customers when sending specific emails, tag them. Add the **Add customer tags** action to label the customer as "New." Once tagged, the customer will remain in the **"New"** category for the next 6 months.

![](https://cdn.heymantle.com/docs/screenshots/3011b49a-7771-4c52-9179-f0dd8bc49159/customer-workflow_1dm63wx.png)

## Organize customers by their email domains and countries

Organizing customers by country can significantly simplify product recommendations. To detect a customer's country or email domain and determine which marketing materials to send, you can sort customers from the USA and Europe as follows:

1.  Start with the **Customer created** trigger.
2.  Select the **Email** condition → then select **ends with** → and set it equal to **".com"**.
3.  Tag these customers with "USA" and use **Send email** to notify yourself.

![](https://cdn.heymantle.com/docs/screenshots/21d03ce6-23d1-4def-b28c-98bd16fbe7c1/organize-customers-by-email_1j66h68.png)

4.  You can also mark customers from Europe → choose the same condition, set the European domain **".eu"**, tag them as "Europe", and **Send email**.

![](https://cdn.heymantle.com/docs/screenshots/15a2310d-0d8e-4fce-83d3-7e94d3429500/organize-customers-by-email-eu_qemuq0.png)

This workflow segments customers by country, allowing you to offer them relevant products that account for their local tax rates.

## Tag special customers and reward them with a discount

Sometimes it's necessary to segment customers into special categories — such as students or employees — to offer them discounts. You can identify their domain or email address and assign a relevant tag.

1.  Start with the **Customer created** trigger.
2.  Verify whether the email contains the ".edu" domain — select the **Email** condition and set **includes .edu**.
3.  Add the **Send email** action to notify yourself about the customer.

![](https://cdn.heymantle.com/docs/screenshots/cc603443-7460-4156-9997-9f1267e54121/provide-educational-discount_1ruhxae.png)

4.  Add one more condition to identify employee customers → select the same condition → set **ends with** @example.com (the email domain you want to tag) → tag this customer as "employee" and send the email.

![](https://cdn.heymantle.com/docs/screenshots/1e6bc223-7b1c-4a2e-a6c1-6ac2f7c5a48e/provide-discount_csao6d.png)

## Segment new customers with a high conversion intent

New customers who place their first orders within 3 days can be considered high-intent.

This workflow includes the following steps:

1.  The starting trigger is **Order created**.
2.  To verify the customer's order count, scroll down to **Order/Customer** and choose the **Orders count** condition — set it equal to 1.
3.  Add another condition — **Days to conversion** — and set it to less than **3**.

![](https://cdn.heymantle.com/docs/screenshots/e7102093-402e-4962-83fc-fc9e74920d51/segment-customers_1c1nh3p.png)

4.  Add the **"high-intent"** tag and **Update customer note** to record their high intent.

![](https://cdn.heymantle.com/docs/screenshots/2ffa5399-0733-4dee-ba87-34e08ac84256/segment-new-customer_162luun.png)

To save all changes in the described workflows, click the **"Turn on"** button.

## Suggested articles

*   [Most popular flows](/react-flow/most-popular-flows)
*   [Order workflows](/react-flow/order-workflows)
*   [Product workflows](/react-flow/product-workflows)
