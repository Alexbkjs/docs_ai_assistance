---
type: page
title: Components of the workflow
seoTitle: Components of the workflow
seoDescription: Three components of the workflow
slug: components-of-the-workflow
order: 20
status: published
---


# What are the elements of the workflow?

In this guide, you'll find a detailed explanation of what each workflow component means and how it works.

## Three components of the workflow

A workflow consists of three main components that you need to configure to define the exact parameters by which it runs.

**Trigger** — an action performed in your store that launches an automatic workflow (for example, an order was cancelled in your store).

**Condition** — a special factor that determines whether the selected action is performed (when the trigger is selected, you can verify whether the customer whose order was cancelled should be notified).

**Action** — the final result of the workflow, achieved after the triggers and conditions are met (an email notifying the customer about the cancelled order was sent).

## Triggers, conditions, and actions in the workflows

### Setting up Triggers

Triggers are essential elements of a workflow. They are the mechanisms that launch the automatic workflow — specifically, events that occur in your store (e.g., creating a new order or cancelling one). When a trigger event occurs, your workflow starts and performs the defined action.

**Why add triggers?**

When you set up a trigger, you choose an event that has occurred in your store, and the app automatically identifies which actions should follow and what changes will be performed.

**How it works**

Click **"Create workflow"** to start your workflow. Once you've selected a trigger, you'll be able to manage other components such as conditions and actions.

[React Flow Triggers](/en/article/react-flow-triggers-actions-1vwyrbi/#2-react-flow-triggers)

### Setting up Conditions

After setting the trigger, the next step is conditions — important elements that determine whether the final action will be performed once certain criteria are met. Each condition has operators to check whether specific parameters match.

**What do they do?**

Conditions ensure that further actions are performed only after the required criteria are met. If the conditions are not met, the actions will not be executed.

**How it works**

To set up conditions, click the **"Condition"** button and select a condition from the drop-down list in the field on the right.

![](https://cdn.heymantle.com/docs/screenshots/893b1658-229c-4da0-b6c8-bc9682fc520d/add-condition-react-flow_2owgjh.png)

There are two operators — **"Otherwise"** and **"Then"** — that determine further actions.

*   "Otherwise" is used when the condition is not met.
*   "Then" is used when the condition is met.

In both cases, you can add a delay, A/B testing, conditions, and actions.

For example, select the trigger action "Customer created" → click on "then" to select the condition "Customer / Orders / Orders / Customer accepts marketing" to verify whether this customer has agreed to receive your marketing materials.

![](https://cdn.heymantle.com/docs/screenshots/9cd31f67-22eb-4c9d-95fe-726c08ef29cd/customer-accepts-marketing_anglgx.png)

Set a final action — "Add customer tags" — to mark the customer with a tag. If the condition is met, the workflow ends with this action. If not, you can leave the workflow as is or add another condition or action by clicking "Otherwise".

You can add **several** conditions in both scenarios to create **one common** condition by clicking "Add another condition". In this case, the final action will be performed only if all conditions are met. If even one is not satisfied, the action will not be performed.

![](https://cdn.heymantle.com/docs/screenshots/a95d3bc5-eba9-4970-b4f7-e14b3217c5d9/add-several-conditions_1suv6vo.png)

You can add as many actions as you like to complete the workflow by clicking "then" → **"Action"** button.

![](https://cdn.heymantle.com/docs/screenshots/8079d302-9f36-4c25-9f7f-8d369625efb0/add-several-actions_1ky0pvq.png)

### Setting up Actions

Actions are the final step in every workflow — they apply changes to your store. They can be **Shopify** or **External**. Shopify actions make changes inside your store, while external actions handle sending emails or HTTP requests to customers.

###### Shopify actions

These actions make changes inside your store. The available actions vary depending on the selected trigger and can relate to customers, products, collections, orders, payments, and more.

###### External actions

Sometimes you need to contact customers outside your store — for example, via email to inform them about updates. In these cases, use the External actions.

[React Flow Actions](/en/article/react-flow-triggers-actions-1vwyrbi/#2-react-flow-actions)

### Delay your workflow for a better time

Alongside the **"Action"** button, you'll find the **"Delay"** button. This lets you schedule a convenient time for your workflow using the React Flow Delay function. If you don't want it to start immediately after the trigger fires, choose the appropriate time interval.

Click **"Delay"** and configure your delay time.

Select the time type (hours or days) in the **"Select time interval"** field, then set the value — the specific number of hours or days.

![](https://cdn.heymantle.com/docs/screenshots/03339115-f80e-423f-9002-9e858343a130/set-delay_miihxb.png)

## Suggested articles

*   [React Flow Triggers & Actions](/react-flow/react-flow-triggers-actions)
*   [Most popular flows](/react-flow/most-popular-flows)
