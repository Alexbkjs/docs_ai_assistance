---
type: page
title: How does the auto recommendation work?
seoTitle: How does the auto recommendation work?
seoDescription: What is an automatic offer?
slug: how-does-the-auto-recommendation-work
order: 13
status: published
---


# What is an automatic offer?

An **automatic offer** lets merchants display product recommendations to customers automatically, immediately after a purchase. The offer is based on the items in the customer's cart and shows products related to what they bought.

Example: when a customer buys a bike, the app may automatically suggest a **bike helmet** as a post-purchase upsell — though this **depends on several factors**.

Shopify has built-in functionality for [determining recommendations](https://shopify.dev/docs/themes/product-merchandising/recommendations), and ReSell relies on this for automatic offers.

![](https://cdn.heymantle.com/docs/screenshots/7164fef4-5889-4c12-95b8-bd36b3d12329/automatic-offer_1wawsp9.png)

## How Shopify recommendations work

There are two types of recommendations:

*   **Related recommendations** — the platform suggests a mix of products that are similar or complementary to the product the customer is viewing. These recommendations are generated automatically by Shopify.
*   **Complementary recommendations** — Shopify suggests products that complement a specific product the customer is viewing. These must be [manually set up](https://help.shopify.com/en/manual/online-store/search-and-discovery/product-recommendations).

You can configure both types of recommendations for free in the [Shopify Search & Discovery](https://apps.shopify.com/search-and-discovery) app.

![Customizing product recommendations in Search & Discovery app](https://cdn.heymantle.com/docs/screenshots/607f7a58-5df0-4cff-b31b-670f93c05fd3/image_11akpa3.png)

## Recommendation logic

[Recommendation logic](https://shopify.dev/docs/themes/product-merchandising/recommendations#recommendation-logic) is based on purchase history, product description, and related collections.

*   **Purchase history** — finds products that have historically been purchased together.
*   **Product description** — finds products with similar descriptions.
*   **Related collections** — finds products from collections that the current product belongs to, excluding collections with handles `all` and `frontpage`.

Important: we are not responsible for the recommended products. Because product selection is based on Shopify's internal algorithms and Search & Discovery app settings, we cannot control which products are recommended to customers.

## Next step

Check our articles to learn more about the app's functionality:

*   [Is there a limit on customer orders?](/resell/is-there-a-limit-on-customer-orders)
*   [Can I customize my offers?](/resell/can-i-customize-my-offers)
