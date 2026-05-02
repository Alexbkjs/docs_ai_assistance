---
type: page
title: Run Code
seoTitle: Run Code
seoDescription: ""
slug: run-code
order: 46
status: published
---


# Run Code

## About the Run Code action

The Run Code action enables you to insert JavaScript blocks into your workflow, giving you complete control over logic, data transformation, and integration with Shopify's API. It is ideal for advanced users who need more flexibility than what standard Flow blocks offer.

## Key Benefits

**1\. Flexible Logic**

Build custom logic that goes beyond the capabilities of standard workflow blocks. Whether it's conditional branching, calculations, or complex data processing, the Run Code action handles it all.

**2\. JavaScript in Your Workflow**

Use familiar JavaScript syntax to manipulate data, access variables, and define how your automation should behave. Compared to Liquid, JavaScript offers far more capabilities, making it easier to implement dynamic logic.

**3\. Access Additional Data**

The Run Code action allows you to fetch and return extra data from the Shopify API, even data that standard React Flow blocks cannot access. You can then use this information as variables or conditions in subsequent steps of your workflow.

**4\. Advanced Automation Scenarios**

Handle complex or non-standard automation tasks without relying on external systems or complicated workarounds. This unlocks new levels of control and efficiency in your store's operations.

## Workflow Example

Example: You want to assign the appropriate tag to a customer whose last 20 orders total more than $5,000.

1.  Open the app and click **Create new** → Create from scratch.
2.  Click **View templates** in the Run Code block and select the "**Tag customer by spend across the last 20 orders**" template.

![](https://cdn.heymantle.com/docs/screenshots/0d6f1406-118c-407b-830d-605f26872452/run-code-action_1hwooia.png)

3.  Configure the template according to your needs. For example, you can adjust the threshold value or add more conditions. Then go to the Add customer tag action and set the required tags.

![](https://cdn.heymantle.com/docs/screenshots/ad1bd283-9310-4952-a4c1-f1e92e530a10/run-code-add-customer-tag_5dj3m.png)

4.  **Save** the workflow.

You can click **Run test** to check how this workflow executes. Click **Turn on** when you are ready to activate it.

## Next Step

This article provides a general overview of the Run Code functionality. For technical details, see the dedicated [Run Code Technical Guide](/react-flow/run-code-technical-guide).
