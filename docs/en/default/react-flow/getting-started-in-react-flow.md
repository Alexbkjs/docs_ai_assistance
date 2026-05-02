---
type: page
title: Getting started in React Flow
seoTitle: Getting started in React Flow
seoDescription: How to start in React Flow?
slug: getting-started-in-react-flow
order: 39
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# Getting started in React Flow

# Quick start in React Flow

  

****In this article:****

*   [How to start in React Flow?](#1-how-to-start-in-react-flow)
*   [Steps to create your first workflow](#1-steps-to-create-your-first-workflow)
*   [The result of the workflow](#1-the-result-of-the-workflow)

  

# ✔️ How to start in React Flow?

  

To start using React Flow you just need to Add app from the Shopify App Store, then, click on it in the app list and open a Dashboard. Here you can start createing your workflows.

  

On the Dashboard you will see all your workflows in the ****“All”**** section, activated ones in the ****“On”****, and deactivated in the ****“Off”****.

  

![React Flow Dashboard](https://cdn.heymantle.com/docs/screenshots/a7fbfdbe-8aca-4085-92bb-5beb9291ac18/react-flow-dashboard_1ngxeq3.png)

  

# ✔️ Steps to create your first workflow

  

## React Flow allows you to create and customize your own workflow that will fit your needs.

  

A workflow is an automatic sequence of actions aimed at performing daily tasks in your store. To put all your routine work to automatic mode, the first thing you need to do is to create a workflow.

  

Let's take for example this business ****problem****: a store owner wants to sort out the customers and create relevant categories to build the right communication with them in the future. Thanks to this, the store owner will have 3 separate categories of customers (****Gold****, ****Silver****, and ****Bronze****), based on the average order amount, which will allow him to offer the most relevant products and send marketing materials further.

  

So, the best solution for this problem is to create a workflow that will mark these customers with special ****tags**** by which it will be easy to find them in the future.

  

### Here are the necessary steps to follow:

  

1.  ****Step 1.**** To start your first workflow you need to click on the ****“Сreate new****” button at the top right to create a proper one and fit it to your needing.

  

![Create your first workflow](https://cdn.heymantle.com/docs/screenshots/88172cc7-b2bf-45c2-94c9-26e9c51857e0/create-your-first-workflow_dk0k5x.png)

  

2.  ****Step 2.**** You will be moved to the workflow builder area where you can start creating and customizing your workflow. For this, in the right menu you should select a trigger to define when the workflow will start.

  

For our workflow, we need to set the \*\*"Order paid" \*\*trigger that will launch it. This trigger will launch further automatic processes when the customer has already made a purchase (paid) in his store.

  

3.  ****Step 3.**** When the trigger is selected, we should set up a condition before the final action to establish certain rules by which the final action will be carried out. Click on plus -> click ****"Condition"****, then select one from the drop-down list on the right.

  

Let's select a condition to verify if the order amount is $750 or more. In the drop-down list of all order conditions go down to the ****"Order / Customer / Amount spent / Average order amount"**** block.

  

![](https://cdn.heymantle.com/docs/screenshots/ebf0a744-c7dc-42a9-aaf8-90a15261d5bb/select-order-customer-conditio_20iain.png)

  

Then, in the field on the right select the matcher ****greater than or equal to**** and write the value "750". Now, with this condition, he will track the orders with this amount.

  

![](https://cdn.heymantle.com/docs/screenshots/484b4ddc-653c-47fb-9fc2-81b4bf1767b4/set-condition_dzrq1w.png)

  

4.  ****Step 4.**** After this, let's add an action to end the workflow. Let's click on plus near ‘then’ and select Action to choose the necessary action which will be performed after the trigger and condition are met. In our case, we need to select the ****"Add customer tags"**** action and write ****GOLD**** in the field on the right.

  

![](https://cdn.heymantle.com/docs/screenshots/95bdb329-54d9-4164-a6a2-8ea9b0805993/add-customer-tags_xqaqnq.png)

  

This action will mark the customers with a ****"GOLD"**** tag. Thanks to this action, such customers will be placed in a "gold" category as VIP clients.

  

If the condition isn't met, we should add another condition by clicking on plus near “otherwise” and selecting ‘Condition’ to track the customers whose order amount is less than $750 and more than $500. For this case we add the same condition as in the previous example and set the value "500".

  

But we also need to specify that the order amount should be less than "750" and equal or more than "500".

  

React Flow allows you to combine conditions to make a common one. It can be done by clicking the ****"Add another condition"**** button below the first condition.

  

For our workflow we select the same condition. And here we should set ****"less than"**** matcher and write "750".

  

![](https://cdn.heymantle.com/docs/screenshots/9654821b-2c28-49eb-ba8e-71df69d28c1f/add-new-conditions_rjuvhi.png)

  

Also, we need to select one more action to mark this customer with another tag. To do this, we click on plus near ‘then’ -> select Action -> select an action ****"Add customer tags"**** and write ****"SILVER"****.. Now, these customers will be placed in the "silver" category.

  

![](https://cdn.heymantle.com/docs/screenshots/d336de53-f2dc-41ec-9b1f-b3bb60348530/add-action-to-condition_1rx04d6.png)

  

5.  ****Step 5.**** Finally, if the previous condition isn't met, we should add another action to set the tag ****"BRONZE"**** for all other customers.

  

![](https://cdn.heymantle.com/docs/screenshots/51b83126-1b44-4c11-8a07-a0106ad4041e/customer-tag-workflow_19o62a4.png)

  

6.  ****Step 6.**** When all is set click on ****“Save”**** on the top "Unsaved changes" panel and set a workflow’s title.

  

  

7.  ****Step 7.**** Finally, your workflow is ready to run after clicking the \*\*“Turn on” \*\*button on the top panel.

  

  

# ✔️ The result of the workflow

  

Having run an automatic workflow the store owner already got rid of spending extra hours on tracking orders and sorting customers by yourself. Now, he has 3 different categories of customers and clearly understand its audience which means he will hit the right target with product and marketing selection.

  

Now, you can start your first automatic workflow too! Focus on the important things while React flow is doing all necessary work for you!

  

  

## Suggestion articles

  

*   [Most popular flows](/most-popular-flows)
*   [React Flow Triggers & Actions](/react-flow-triggers-actions)
*   [Guidelines & Limitations](/guidelines-and-limitations)

  

  

Updated on: 16/10/2025