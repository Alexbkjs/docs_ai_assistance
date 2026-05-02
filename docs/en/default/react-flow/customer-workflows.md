---
type: page
title: Customer Workflows
seoTitle: Customer Workflows
seoDescription: What are the Customer workflows?
slug: customer-workflows
order: 25
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# Customer Workflows

  

# Customer Workflows

  

****In this article:****

  

[What are the Customer workflows?](#1-what-are-the-customer-workflows)

*   [1\. Send a thank-you email to a new customer and build his loyalty](#2-send-a-thank-you-email-to-a-new-customer-and-build-his-loyalty)
*   [2\. Organize customers by their email domains and countries](#2-organize-customers-by-their-email-domains-and-countries)
*   [3\. Tag special customers and reward them with a discount](#2-tag-special-customers-and-reward-them-with-a-discount)
*   [4\. Segment new customers that have a high conversion intent](#2-segment-new-customers-that-have-a-high-conversion-intent)

# ✔️ What are the Customer workflows?

  

Building trust with customers is a top priority for any business owner, as it is the foundation for future growth. Throughout the day, it's essential to maintain effective communication and address various issues, such as shipping, refunds, email correspondence, and risk verification.

  

For this category, there are some triggers that can run the workflows:

  

*   Customer created
*   Customer deleted
*   Customer account enabled
*   Customer account disabled

  

In this help guide, we are going to consider some examples of workflows for the ****"Customers"**** category.

  

## Send a thank-you email to a new customer and build his loyalty

  

1.  Start with the ****Customer created**** trigger
2.  Verify if this customer agreed to accept marketing materials and you can use his email for that → Select the ****Accepts marketing**** condition and set "is true"
3.  Once a new customer has joined our store, we want to send him an email with a 3-days gift coupon that he can use as a new member. → So, we should set a ****Delay**** of 1 day before the ****Send email**** action.
4.  To quickly identify new customers when you need to send them specific emails, it's helpful to tag them. Simply add the ****Add customer tags**** action to label the customer as "New." Once tagged, this customer will remain in the ****"New"**** category for the next 6 months.

  

![](https://cdn.heymantle.com/docs/screenshots/3011b49a-7771-4c52-9179-f0dd8bc49159/customer-workflow_1dm63wx.png)

  

## Organize customers by their email domains and countries

  

Organizing customers by countries can significantly simplify the product recommendations for them. That's why we need to detect their country or email domain to know exactly what marketing materials to send. In this case, we need to sort out the customers who are located in the USA and in Europe:

  

1.  We start with the ****Customer created**** trigger.
2.  Next, we need to select the ****Email**** condition → then, select ****ends with**** → and set is equal to ****".com"****.
3.  When we've detected the email domain we need to tag these customers with the "USA" tag and ****Send email**** to get notified about him.

  

![](https://cdn.heymantle.com/docs/screenshots/21d03ce6-23d1-4def-b28c-98bd16fbe7c1/organize-customers-by-email_1j66h68.png)

  

4.  We can also mark other customers from Europe → we choose the same condition and set the European domain ****".eu"**** , tag them as "Europe", and ****Send email****.

  

![](https://cdn.heymantle.com/docs/screenshots/15a2310d-0d8e-4fce-83d3-7e94d3429500/organize-customers-by-email-eu_qemuq0.png)

  

This workflow segments customers by their countries which allows us to offer them the relevant products considering the tax rates of their country.

  

## Tag special customers and reward them with a discount

  

Sometimes, it's necessary to segment customers into special categories, such as students or employees, to offer them discounts. To do this, we can identify their domain or email address and assign a relevant tag.

  

1.  This workflow starts with the ****Customer created**** trigger
2.  We verify if his email contains the ".edu" domain. Select the ****Email**** condition and set ****includes .edu****
3.  Then, add the ****Send email**** action to get notified about the customer.

  

![](https://cdn.heymantle.com/docs/screenshots/cc603443-7460-4156-9997-9f1267e54121/provide-educational-discount_1ruhxae.png)

  

4.  Let's add one more condition to get notified about the employee customer → select the same condition → set the ****ends with**** @example.com - the email domain that you need to tag → Tag this customer as "employee" and send the email.

  

![](https://cdn.heymantle.com/docs/screenshots/1e6bc223-7b1c-4a2e-a6c1-6ac2f7c5a48e/provide-discount_csao6d.png)

  

## Segment new customers that have a high conversion intent

  

If there are new customers who have placed their first orders in less than 3 days they can be considered as high-intent to conversions.

  

This workflow will contain the following steps:

  

1.  The starting trigger is ****Order created****
2.  To verify the amount of orders of the customer, scroll down to the ****Order/Customer**** and choose the ****Orders count**** condition - set is equal 1
3.  Add another condition - ****Days to conversion**** - and set less than ****3****.

  

![](https://cdn.heymantle.com/docs/screenshots/e7102093-402e-4962-83fc-fc9e74920d51/segment-customers_1c1nh3p.png)

  

4.  Add the ****"high-intent"**** tag and ****Update customer note**** that informs about their high intent

  

![](https://cdn.heymantle.com/docs/screenshots/2ffa5399-0733-4dee-ba87-34e08ac84256/segment-new-customer_162luun.png)

  

To save all the changes in the described workflows, click the " ****Turn on****" button.

  

## Suggested articles

  

*   [Most popular flows](/most-popular-flows)
*   [Order workflows](/order-workflows)
*   [Product workflows](/product-workflows)

  

Updated on: 25/03/2026