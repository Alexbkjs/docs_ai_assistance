---
type: page
title: Why is my Post-purchase upsell offer not displayed?
seoTitle: Why is my Post-purchase upsell offer not displayed?
seoDescription: You can check the Shopify article about limits and considerations for post-purchase checkout extentions for detailed information on restrictions.
slug: why-is-my-post-purchase-upsell-offer-not-displayed
order: 2
status: published
---


# Reasons Why a Post-purchase Offer Is Not Displayed

You can check the Shopify article on [limits and considerations for post-purchase checkout extensions](https://shopify.dev/docs/apps/checkout/product-offers/post-purchase#limitations-and-considerations) for detailed information on restrictions.

Below are the most common reasons an offer may not be displayed.

###### Unsupported Payment Methods

The following payment methods are not supported for post-purchase upsells due to Shopify's limitations:

*   **Installment/Buy Now, Pay Later services**: including Affirm, AfterPay, Shop Pay Installments, Sezzle, Klarna, and similar services.
*   **Unsupported payment wallets**: Apple Pay, Amazon Pay, Google Pay, PayPal Wallet.
*   **Bank transfer payment methods**: iDeal.

###### Common reasons why offers are not displayed

*   Your store is multi-currency and the order is placed in a currency different from the store currency.
*   ReSell is not enabled as your post-purchase page app in the Checkout settings.
*   The order total is under $0.50, or the order is paid with a gift card or cash on delivery (COD).
*   Both the product in the original order and the upsell product are subscription products.
*   The product's inventory is tracked and the available quantity is zero or less.
*   The product has been ordered for local delivery.
*   [Automatic payments](/resell/how-to-connect-paypal-to-shopify) are disabled while using PayPal Express Checkout.
*   The Shopify platform is temporarily overloaded.

###### What should you do if orders come from unsupported payment methods?

If your store frequently receives orders via unsupported payment methods — such as Buy Now, Pay Later services or regional options like Razorpay or Airwallex — we recommend using **Thank you page offers** as an alternative. These can still help increase conversions even when standard post-purchase offers cannot be shown.

If you have checked all the items above and your offer is still not appearing, please contact our support team: [support@devit.software](mailto:support@devit.software).

Please note that Shopify supports the following payment methods: Shopify Checkout, PayPal Pro, PayPal PayFlow, Braintree, [Shop Pay](https://www.shopify.com/blog/shop-pay-checkout), and [PayPal Express](https://help.shopify.com/en/manual/payments/paypal).

If you use PayPal, make sure your store is approved for [PayPal Automatic payments](https://help.shopify.com/en/manual/payments/paypal/set-up-paypal#:~:text=If you're using a post-purchase upsell app%2C then Shopify shows PayPal as a payment option during checkout%2C even if you're not yet approved for Reference Transactions with PayPal%2C but post-purchase offers aren't shown to the customer).

Please also note that Shopify only supports vaulted card payment processors. For more information, refer to this article: [Vaulted payment processors](/resell/vaulted-payment-processors).

## Next step

Check our articles to learn more about the app's functionality:

*   [How does the post-purchase upsell offer affect my fulfillment?](/resell/how-does-the-post-purchase-upsell-offer-affect-my-fulfillment)
*   [Which payment method is supported by ReSell?](/en/article/which-payment-method-is-supported-by-resell-191jn6k/)
