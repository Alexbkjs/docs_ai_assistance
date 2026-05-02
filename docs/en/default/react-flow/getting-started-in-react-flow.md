---
type: page
title: Getting started in React Flow
seoTitle: Getting started in React Flow
seoDescription: How to start in React Flow?
slug: getting-started-in-react-flow
order: 39
status: published
---


# Quick start in React Flow

## How to start in React Flow?

To start using React Flow, add the app from the Shopify App Store, click on it in the app list, and open the Dashboard. From here, you can start creating your workflows.

On the Dashboard, you'll see all your workflows in the **"All"** section, activated ones under **"On"**, and deactivated ones under **"Off"**.

![React Flow Dashboard](https://cdn.heymantle.com/docs/screenshots/a7fbfdbe-8aca-4085-92bb-5beb9291ac18/react-flow-dashboard_1ngxeq3.png)

## Steps to create your first workflow

React Flow lets you create and customize workflows tailored to your needs.

A workflow is an automatic sequence of actions designed to handle daily tasks in your store. To put your routine work on autopilot, the first step is to create a workflow.

Let's use this business **problem** as an example: a store owner wants to categorize customers and create relevant groups for better future communication. The goal is to create 3 customer categories — **Gold**, **Silver**, and **Bronze** — based on average order amount, which will allow offering the most relevant products and sending targeted marketing materials.

The best solution is to create a workflow that tags these customers so they can be easily found later.

### Steps to follow:

1.  **Step 1.** Click the **"Create new"** button in the top-right corner to create your first workflow.

![Create your first workflow](https://cdn.heymantle.com/docs/screenshots/88172cc7-b2bf-45c2-94c9-26e9c51857e0/create-your-first-workflow_dk0k5x.png)

2.  **Step 2.** You'll be taken to the workflow builder, where you can start creating and customizing your workflow. In the right-side menu, select a trigger to define when the workflow starts.

For this workflow, set the **"Order paid"** trigger, which fires when a customer completes a purchase.

3.  **Step 3.** With the trigger selected, set up a condition to establish the rules for the final action. Click plus → click **"Condition"**, then select one from the drop-down list on the right.

Select a condition to verify whether the order amount is $750 or more. In the drop-down list, navigate to the **"Order / Customer / Amount spent / Average order amount"** block.

![](https://cdn.heymantle.com/docs/screenshots/ebf0a744-c7dc-42a9-aaf8-90a15261d5bb/select-order-customer-conditio_20iain.png)

Then, in the field on the right, select the **greater than or equal to** matcher and enter the value "750".

![](https://cdn.heymantle.com/docs/screenshots/484b4ddc-653c-47fb-9fc2-81b4bf1767b4/set-condition_dzrq1w.png)

4.  **Step 4.** Next, add an action to complete the workflow. Click plus near "then" and select **Action** to choose the action that runs when the trigger and condition are met. Select **"Add customer tags"** and enter **GOLD** in the field on the right.

![](https://cdn.heymantle.com/docs/screenshots/95bdb329-54d9-4164-a6a2-8ea9b0805993/add-customer-tags_xqaqnq.png)

This action tags customers with **"GOLD"**, placing them in a VIP category.

If the condition isn't met, add another condition by clicking plus near "otherwise" and selecting "Condition" to track customers whose order amount is less than $750 but more than $500. Add the same condition type and set the value "500".

You also need to specify that the order amount should be less than "750" and equal to or more than "500".

React Flow lets you combine conditions into a single composite condition by clicking **"Add another condition"** below the first condition.

For this workflow, select the same condition type, set the **"less than"** matcher, and enter "750".

![](https://cdn.heymantle.com/docs/screenshots/9654821b-2c28-49eb-ba8e-71df69d28c1f/add-new-conditions_rjuvhi.png)

Add one more action to tag this customer. Click plus near "then" → select **Action** → select **"Add customer tags"** and enter **"SILVER"**. These customers will be placed in the "silver" category.

![](https://cdn.heymantle.com/docs/screenshots/d336de53-f2dc-41ec-9b1f-b3bb60348530/add-action-to-condition_1rx04d6.png)

5.  **Step 5.** Finally, if the previous condition isn't met, add one more action to assign the **"BRONZE"** tag to all remaining customers.

![](https://cdn.heymantle.com/docs/screenshots/51b83126-1b44-4c11-8a07-a0106ad4041e/customer-tag-workflow_19o62a4.png)

6.  **Step 6.** When everything is set, click **"Save"** on the top "Unsaved changes" panel and give the workflow a title.

7.  **Step 7.** Your workflow is ready. Click the **"Turn on"** button on the top panel to activate it.

## The result of the workflow

With this automatic workflow, the store owner no longer spends extra hours tracking orders and sorting customers manually. They now have 3 distinct customer categories and a clear understanding of their audience, enabling more targeted product and marketing decisions.

Now you can start your first automatic workflow too — focus on what matters while React Flow handles the routine.

## Suggestion articles

*   [Most popular flows](/react-flow/most-popular-flows)
*   [React Flow Triggers & Actions](/react-flow/react-flow-triggers-actions)
*   [Guidelines & Limitations](/react-flow/guidelines-and-limitations)
