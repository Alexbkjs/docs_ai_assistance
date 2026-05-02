---
type: page
title: React Flow Counters
seoTitle: React Flow Counters
seoDescription: What are counters?
slug: react-flow-counters
order: 2
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# React Flow Counters

# React Flow Counters

****In this article:****

*   [What are counters?](#1-what-are-counters)
*   [An example from templates?](#1-an-example-from-templates)
*   [How to count how many people used the discount?](#1-how-to-count-how-many-people-used-the-discount)
*   [How to calculate how many products were bought with a tag HOT in a week?](#1-how-to-calculate-how-many-times-a-week-hot-tag-products-are-ordered)

<iframe type="text/html" width="560" height="349" src="https://www.youtube.com/embed/b5Fg7KBC590?rel=0" loading="lazy" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; border: 0px;"></iframe>

# ✔️What are counters?

With the help of counters, you can develop scenarios that will help improve your store automation. The counter allows you to manage data calculations that can then be used in managing your store.

# ✔️An example from templates

One of the examples of using counters can be located in the Templates tab. Let's check it out together.

First, choose ****Tag HOT products**** template. It can help you identify and tag products that are purchased throughout the day. If a given product is also purchased the next day, the tag HOT stays in its place, but if not - the tag is automatically removed.

![](https://cdn.heymantle.com/docs/screenshots/85b47081-12cb-4daa-8cf1-c2c71e9e8ddf/znimok-ekrana-2022-11-14-o-001_1ixxdkq.png)

# ✔️How is this template implemented?

1.  ****Step 1.**** ****Order line item created**** is a specific trigger that allows you to interact with a specific product and not with the entire order. If this event has occurred, it means that the product has been bought and has to be assigned a tag.
    
2.  ****Step 2.**** Now, you need to set up a counter to understand whether a product was purchased throughout the day. This action has already been integrated into the template. Pay attention to the name of the counter. The respective variable specified in the template allows you to dynamically name the counter, whereas each product will have its own ID. In other words, you will have a separate counter for each product.
    

![](https://cdn.heymantle.com/docs/screenshots/836ae928-fc40-4b0f-818b-381c7d3c5be8/change-counter-action_1xnhhzm.png)

✅ You can use action ****Change trigger**** in any workflow chain, you can count literally anything in your store.

3.  ****Step 3.**** Since the moment of purchase, let’s set a delay, say of 24 hours. If the counter has not been modified in the last 24 hours, then the tag should be removed

![](https://cdn.heymantle.com/docs/screenshots/67a9e2d7-3b14-4e51-af5d-8ce4015e410e/order-line-item-created-workfl_dfkbca.png)

4.  ****Step 4.**** If a certain product is bought daily, the counter will change without the tag being removed. You can adjust the conditions according to your needs. For example, change the time period after which the counter will be updated.

![](https://cdn.heymantle.com/docs/screenshots/75c4b480-b987-4678-94c0-e6c58b710d63/counter-updated_13mg8ou.png)

Counters are a flexible solution that allows you to implement almost any calculation you need, such as setting the counter as weekly and receiving the required reports.

# ✔️How to count how many people used the discount?

And to finish it up with another example. You might want to count how many people have used a gift certificate in your shop. To do this with the counter function, follow these steps:

1.  ****Step 1.**** Select trigger ****Order created.****
2.  ****Step 2.**** Add condition ****Order/discount.****
3.  ****Step 3.**** Choose the matcher ****Is equal.****
4.  ****Step 4.**** Write in line ****Value**** name of discount code.

![](https://cdn.heymantle.com/docs/screenshots/750f5a7f-dc26-426b-a4ab-a89404bc43f8/discount-code_10gtidu.png)

5.  ****Step 5.**** Then add action ****Change counter**** and give a name to this counter.

![](https://cdn.heymantle.com/docs/screenshots/71d91028-954b-49d8-9691-df6e54788e8e/change-discount-counter_q8kvdn.png)

If you wish, you can configure the sending of a letter to your email address and then reset the counter.

# ✔️How to calculate how many times a week hot tag products are ordered???

Let's count how often are products with the HOT tag are ordered in a week. We will configure sending an email to the store owner and resetting the counter. You need to reset the counter so that every week it starts counting from the beginning and you see the numbers for a specific week.

1.  ****Step 1.**** Select trigger ****Order created.****
2.  ****Step 2.**** Add condition ****Order/Line items.****
3.  ****Step 3.**** Select the matcher ****Any of line items matches the following**** and select ****Line items/product tags**** -> ****Includes**** -> set the value ****HOT**** . Now we can count how many products with the tag ****HOT**** were bought in a week.

![](https://cdn.heymantle.com/docs/screenshots/cbd047d3-be8c-4682-8ae1-e647b32aed0b/order-created-line-items_194pa73.png)

3.  ****Step 4.**** Add action ****Change counter**** and give a name to this counter.

![](https://cdn.heymantle.com/docs/screenshots/bdcbc94b-4b57-4f0a-b4ab-2503264c20d5/lineitem-change-counter_jmxvgu.png)

Now you need to configure the sending of the letter to your mail address and the automatic reset of the counter every week. You can set up a separate flow for this.

8.  ****Step 8.**** Choose ****Time of week**** as a trigger.
9.  ****Step 9.**** Then ****Send email.****
10.  ****Step 10.**** In the text field add variable ****Counter name.****

![](https://cdn.heymantle.com/docs/screenshots/5afdbfaf-6d66-4c18-a4a9-336d4fa7f73d/time-of-week-counter_tg6y5n.png)

11.  ****Step 11.**** Add a delay of 5 minutes.
12.  ****Step 12.**** Finally сonfigure counter reset.

![](https://cdn.heymantle.com/docs/screenshots/a71b996a-d719-43b5-bab4-8a207a0810cb/change-counter-time-of-week_o619dy.png)

With this flow, you've set up automatic email sending and counter resets to count the total number of products purchased with the tag HOT.

## Suggested articles

*   [Components of the workflow](/components-of-the-workflow)
*   [React Flow Templates](/react-flow-templates)
*   [Most Popular Flows](/most-popular-flows)

Updated on: 25/03/2026