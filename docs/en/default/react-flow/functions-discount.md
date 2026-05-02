---
type: page
title: Functions - Discount
seoTitle: Functions - Discount
seoDescription: About Discount Function
slug: functions-discount
order: 35
status: published
---


# Discount Function

## About Discount Function

A [<u><span style="white-space:pre-wrap" class="csh-markdown csh-markdown-underline">Discount Function</span></u>](https://shopify.dev/docs/apps/build/discounts/build-discount-function?extension=rust) is a custom discount created using Shopify Functions that can be applied to different parts of the checkout process, including cart line items, the order subtotal, or shipping rates.

## Use templates

Before you start creating workflows, we recommend checking the list of available Discount Functions. You may find a suitable template and add the function without extra configuration.

1.  Open the app and go to the **Function** tab in the left-side menu.
2.  Find the **Discount** block and click **Create**.
3.  Click **Create from template**.

![](https://cdn.heymantle.com/docs/screenshots/d82653ec-ad7d-4ba4-8224-ea755c77dd08/functions-template_tbdojq.png)

Select the template you need. Check the settings, apply changes if needed, and click **Save** in the upper-right corner.

You can now see the **Turn on** button in the upper-right corner. Click it to test the workflow.

## Create from scratch

**Example:** Offer a discount when the total amount of items in the cart exceeds 100.

1.  Open the app and go to the **Function** tab in the left-side menu.
2.  Find the **Discount** block and click **Create** → **Create from scratch**.

![](https://cdn.heymantle.com/docs/screenshots/48528780-4ca4-45ac-beb0-037e90fc1f31/functions-from-scratch_18go5p0.png)

3.  Select **Cart line discount** in the right-side menu. Here you can set the start date and time, end date and time, and combinations by selecting additional options.
4.  Click the + icon and select **Conditions**.
5.  Click the **Select conditions** field → Cart → Lines → Cost → Total amount → Amount.

![](https://cdn.heymantle.com/docs/screenshots/f42e46df-4147-41b7-9bc9-e748fcce834e/total-amount-function_1jutvv8.png)

6.  In the **Select matcher** field, select **"greater than"** and set the amount you need.
7.  Click + and select **Action**. Click **Order discount** and set the discount value.
8.  **Save** your workflow by clicking the button in the upper-right corner.

![](https://cdn.heymantle.com/docs/screenshots/00b133a2-655e-4834-8a08-d31e709a836f/order-discount-action_18nio0m.png)

You can now see the **Turn on** button in the upper-right corner. Click it to test the workflow.

## Need help?

Don't worry if this feels technical — our support team can guide you through the process or even set up the function for you. Just send us a message: [<u><span style="white-space:pre-wrap" class="csh-markdown csh-markdown-underline">support@devit.software</span></u>](http://support@devit.software)
