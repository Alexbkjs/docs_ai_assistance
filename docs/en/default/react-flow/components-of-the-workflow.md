---
type: page
title: Components of the workflow
seoTitle: Components of the workflow
seoDescription: Three components of the workflow
slug: components-of-the-workflow
order: 20
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# Components of the workflow

  

# What are the elements of the workflow?

  

****In this article:****

*   [Three components of the workflow](#1-three-components-of-the-workflow)
*   [Triggers, conditions & actions in the workflows](#1-triggers-conditions-and-actions-in-the-workflows)
*   [Setting up Triggers](#3-setting-up-triggers)
*   [Setting up Conditions](#3-setting-up-conditions)
*   [Setting up Actions](#3-setting-up-actions)
*   [Delay your workflow for a better time](#3-delay-your-workflow-for-a-better-time)

  

In this help guide, you’ll find a detailed explanation of what each workflow component means and how it works.

  

# ✔️ Three components of the workflow

  

A workflow consists of three main components that you need to set up to give it the exact parameters by which it will run.

  

****Trigger**** - an action performed in your store that launches an automatic workflow (for example, an order was canceled in your store).****Condition**** - a special factor that determines if the selected action is performed (when the trigger is selected you can verify if the customer whose order was canceled can be notified about it).****Action**** - the final result of the workflow, achieved after the triggers and conditions are met (an email with the notification about the canceled order was sent to the customer).

  

# ✔️ Triggers, conditions, and actions in the workflows

  

### Setting up Triggers

  

Triggers are essential elements in the workflow. These are the mechanisms that launch the automatic workflow. Such mechanisms are the events performed in your store (e.g., creating a new order or canceling it, etc.). When the trigger event occurs, your workflow starts and performs the defined action.

  

****Why add triggers?****

  

When you set up a trigger you choose an event that has occurred in your store and the app automatically identifies which actions should follow next and what changes will be performed.

  

****How it works?****

  

Click on ****“Create workflow”**** to start your workflow. As soon as you’ve selected the trigger you’ll be able to manage other components as conditions and actions.

  

[React Flow Triggers](/en/article/react-flow-triggers-actions-1vwyrbi/#2-react-flow-triggers)

### Setting up Conditions

  

When the trigger is set, next are conditions - important elements that determine whether the final action will be performed if some conditions are met. Each condition has operators to check if certain parameters match.

  

****What do they do?****

  

The conditions make sure that further actions are performed only after the necessary conditions are met. If such conditions are not met, the actions will not be executed.

  

****How it works?****

  

To set up conditions you should click on the ****“Condition”**** button and select the condition from the drop-down list in the field on the right.

  

![](https://cdn.heymantle.com/docs/screenshots/893b1658-229c-4da0-b6c8-bc9682fc520d/add-condition-react-flow_2owgjh.png)

  

There are two operators - ****“Otherwise”**** and ****“Then”****\- that determine further actions.

  

*   “Otherwise” scenario is used when the condition is not met.
*   “Then” scenario is used when the condition is met.

  

In both cases you can add delay, A/B testing, conditions and actions.

  

For example, let's select the trigger action - “Customer created” -> Click on ‘then’ to select condition - “Customer / Orders / Orders / Customer accepts marketing” to verify if this customer has agreed to receive your marketing materials.

  

![](https://cdn.heymantle.com/docs/screenshots/9cd31f67-22eb-4c9d-95fe-726c08ef29cd/customer-accepts-marketing_anglgx.png)

  

Set a final action - “Add customer tags” to mark such customer with a tag. If the condition is satisfied the workflow will end with this action. In case it is not, you can either leave this workflow like this or add another condition or action by clicking “Otherwise”.

  

You can add ****several**** conditions in both scenarios to create ****one common**** condition that should be met by clickin the "Add another condition". In this case, your final action will be performed if all these conditions are met. If even one of them is not satisfied the action won’t be performed.

  

![](https://cdn.heymantle.com/docs/screenshots/a95d3bc5-eba9-4970-b4f7-e14b3217c5d9/add-several-conditions_1suv6vo.png)

  

You can add as many actions as you like to end this workflow by clicking on 'then" -> ****"Action"**** button.

  

![](https://cdn.heymantle.com/docs/screenshots/8079d302-9f36-4c25-9f7f-8d369625efb0/add-several-actions_1ky0pvq.png)

  

### Setting up Actions

  

Actions are the last step in every workflow. They do the final changes in your store. They can be ****Shopify**** and ****External****. The internal actions are the actions that can make changes in your Shopify store, and the external ones regulate the sending of emails or HTTP requests to customers.

  

###### Shopify actions

  

These are the actions that can make changes inside your store. There are different actions that change depending on the selected trigger. They can relate to customers, products, collections, orders, payments, etc.

  

###### External actions

  

Sometimes you need to contact customers outside your shop, so you need to connect with them via email to inform them about some updates in your store. In this case, use the External actions.

[React Flow Actions](/en/article/react-flow-triggers-actions-1vwyrbi/#2-react-flow-actions)

### Delay your workflow for a better time

  

Along with the ****"Action"**** button, you can see the ****"Delay"**** button. Thanks to it, you can plan a convenient time for your workflow with the React Flow Delay function. If you don’t want it to start right after the trigger has fired choose the proper time interval after which it will launch.

  

Click on ****“Delay”**** and configure your delay time.

  

Select the necessary type of time (hours or days) in the field ****“Select time interval”****, and set the value, i.e., the specific number of hours or days.

  

![](https://cdn.heymantle.com/docs/screenshots/03339115-f80e-423f-9002-9e858343a130/set-delay_miihxb.png)

  

## Suggested articles

  

*   [React Flow Triggers & Actions](/react-flow-triggers-actions)
*   [Most popular flows](/most-popular-flows)

  

Updated on: 28/11/2024