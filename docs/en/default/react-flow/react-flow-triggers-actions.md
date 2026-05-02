---
type: page
title: React Flow Triggers & Actions
seoTitle: React Flow Triggers & Actions
seoDescription: React Flow Triggers and Actions&x20;
slug: react-flow-triggers-actions
order: 42
status: published
---


# React Flow Triggers and Actions

In this article, we will tell you about what **Triggers** and **Actions** are and how to use them.

running

Basically, this is the main functionality of the **React Flow** application, which allows you to build various flows to automate processes in your online store,

A workflow consists of main components that you need to set up to give it the exact parameters by which it will run. You can create automated tasks of varying complexity. Multiple **Triggers**, **Conditions**, and **Actions** are available for you.

# React Flow Triggers and Actions

**Triggers** automatically initiate your workflows and can be applied in various scenarios. For example, you can use them to start a flow when a new order is created or successfully paid, a customer registers, a product is added to your store, or even on a specific day and time.

![](https://cdn.heymantle.com/docs/screenshots/edc53941-7c47-4df8-8f38-d8b63d992b5f/react-flow-triggers_egaan2.png)

**Actions** - send well-designed messages to email, tag a customer or an order, work with metafields, publish and unpublish products, automate fulfillment, cancel the order, make a delay between execution, and much more.

![](https://cdn.heymantle.com/docs/screenshots/ba83bcc7-a545-4107-adc1-993c5f8e0c28/actions-react-flow_1r777wv.png)

# How it works?

When you set up a trigger you choose an event that has occurred in your store and the app automatically identifies which actions should follow next and what changes will be performed. First you need to choose a trigger. As soon as you’ve selected it you’ll be able to manage other components as actions. Click **Сreate workflow** to start

![](https://cdn.heymantle.com/docs/screenshots/87366523-0304-40e9-b01b-ecac98d2a53f/create-your-first-workflow_17lr7g5.png)

# Order triggers

The application has **Triggers** that are associated with each component of your store.

In the right column, you can find a **Trigger** that will help optimise your Shopify store: **order created**, **order deleted**, **order cancelled**, **inventory quantity changed**, etc.

With those **Triggers** you can react to certain events related to goods.

![](https://cdn.heymantle.com/docs/screenshots/b677f228-5647-4dbd-a5c0-af03553b7600/order-trigger_11y4kr6.png)

If you choose a **Trigger Order Created** - the workflow starts when the new order is created. Now you can choose **Actions**, **Conditions** or **Delays** for this flow. You can view all **Trigger** options in the column on the right.

![](https://cdn.heymantle.com/docs/screenshots/3d94c60b-3e89-4fd2-88b8-681e2194cdcb/workflow-components_1h5avvf.png)

Let's imagine that you want to capture payment for the order that triggered this workflow - for this you need **Add action Captured payment**.

![](https://cdn.heymantle.com/docs/screenshots/08f41b89-6ad0-42e9-9152-12c848fdc004/capture-payment_1u6g8bl.png)

Or, after the order is created, you can send an order report email with a delay to the customer. Choose **Order created**, add a **Delay** 5 minutes

![](https://cdn.heymantle.com/docs/screenshots/b18e5310-3387-4fc2-b94e-a78c44966b81/set-delay-action_aag2zw.png)

and **Add action Send order report**, add variables to the **Subject** field and write some information for the buyer.

![](https://cdn.heymantle.com/docs/screenshots/a9b46992-267e-4a7f-abbc-394616d8180b/send-order-report_vvo91h.png)

# Customer triggers

Let's look at other groups of **Triggers**, such as related to сustomers.

On the right, you can enter the word: "сustomer" and see the **Triggers** associated with customers.

![](https://cdn.heymantle.com/docs/screenshots/f406d32b-df78-4eb4-b901-39b1c7405bfd/customer-triggers_15xiju8.png)

If you choose one of the **Triggers** such as **Customer created** then you can configure certain actions related to this flow: add a tag and add action. For instance, we can add a tag **New customer**

![](https://cdn.heymantle.com/docs/screenshots/5060ad0d-6baf-4e75-90c2-fbb23217a10f/new-customer-tag_f3tho4.png)

and **Add Action Send new products notification** for customers with this tag. Don't forget to adjust the field on the right so that the letter works best.

![](https://cdn.heymantle.com/docs/screenshots/7810776a-7638-43aa-af76-80717dd0c683/send-new-product-notification_1o2n4el.png)

# Product triggers

Another popular group of triggers is **Product**: Product added to store, Product deleted, Inventory item created (this trigger starts a workflow when a new item was created in your store. The inventory item contains the information about the product’s availability in the stock (if it can shipped), and about its tracking. Also inventory item deleted, Inventory quantity change (this workflow starts if the inventory quantity changes when there is an order created or canceled in your store)

![](https://cdn.heymantle.com/docs/screenshots/9b09aee6-757f-4dbf-895c-bbd363847bac/products-trigger_1c6qazf.png)

# Actions

Once you've decided which trigger to use, you can set up any action. There are different actions that change depending on the selected trigger. They can relate to customers, products, collections, orders, payments, etc - these **Shopify** actions. Or you want to contact your customers to inform about discounts, new collections or clarify the details of the order - there are **External** actions. Also you can find \*\*Connectors. \*\*Read more about Connectors in [this article.](/react-flow/react-flow-connectors)

For instance, for the trigger **Order is created** you can choose **Send order invoice** action or you can Add product variant to order and customise this proposition for your client.'

![](https://cdn.heymantle.com/docs/screenshots/9d755e15-a411-4ff5-83f0-fefc00801718/send-order-invoice_wzahq4.png)

Choose any actions that will help manage processes in your store and communicate with customers

# If you can't find the Trigger or Action you want?

These are just a few of the available **Triggers** and ****Actions \*\*— the app offers extensive functionality. Plus, new \*\*Triggers** and **Actions**** are continuously being added.

If you cannot find the right **Trigger** or **Action** for the situation you want to implement and use in your store - you can write to support and we will try to help you. We are happy to improve our functionality and add new opportunities to optimize your store.

![](https://cdn.heymantle.com/docs/screenshots/040a144d-c419-49df-8df2-2cb768f7927b/help-page_10o0i5a.png)

## Suggestion articles

*   [Order Workflows](/react-flow/order-workflows)
*   [Customer Workflows](/react-flow/customer-workflows)
*   [Product Workflows](/react-flow/product-workflows)

