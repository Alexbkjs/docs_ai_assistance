---
type: page
title: Product Workflows
seoTitle: Product Workflows
seoDescription: What are the Product workflows?
slug: product-workflows
order: 11
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# Product Workflows

# Product Workflows

****In this article:****

*   [What are the Product workflows?](#1-what-are-the-product-workflows)
*   [1\. Get notified of the inventory lack and hide products that are out of stock](#2-get-notified-of-the-inventory-lack-and-hide-products-that-are-out-of-stock)
*   [2\. Organize new products by title and type](#2-organize-new-products-by-title-and-type)
*   [3\. Tag orders that contain products with specific tags](#2-tag-orders-that-contain-products-with-specific-tags)
*   [4\. Delete the product that is out of stock and create a redirect](#2-delete-the-product-that-is-out-of-stock-and-create-a-redirect)
*   [5\. Automatically set product metafield when it is added to store](#2-automatically-set-product-metafield-when-it-is-added-to-store)

# ✔️ What are the Product workflows?

Products are the key elements that attract customers to your store. To enhance their experience, you should offer a well-organized, easy-to-navigate product catalog, sorted by categories. It's also important to notify customers about new products, promote items, and track inventory. Product workflows are designed to simplify and automate these processes, making them more efficient.

## Get notified of the inventory lack and hide products that are out of stock

When the inventory item is low, we need to know about it to restock it with the new products. Let's do this following the next steps:

1.  Start with the ****Inventory quantity changed**** the trigger.
2.  Set the ****Position**** condition to verify if this product is the 31st in the item list → and if the total inventory quantity is ****less than or equal to**** 30.
3.  Then, we should end this workflow by ****adding**** the ****low stock**** tag and sending an email.

![](https://cdn.heymantle.com/docs/screenshots/488c55c0-815a-4128-94d6-ab430b052c8d/inventory-quantity-changed-tri_1f50qcx.png)

4.  When the product has run out of stock, we need to hide it from our store page → Select the ****Total inventory**** condition which is ****less than or equal to**** 0.
5.  Add the final action - ****Hide product****.

![](https://cdn.heymantle.com/docs/screenshots/8fed98d1-b1ed-43dc-9a09-464f916506ff/hide-out-of-stock-product_1fxcvj9.png)

## Organize new products by title and type

There can be a lot of different products that differ in type or title. In the next workflow, we are going to organize them by these two parameters.

### Title

1.  Select the ****Product added to store**** trigger.
2.  Add the ****Title**** condition that ****includes**** title "shoes"
3.  Add the "shoes" ****tag**** and ****add**** this ****product to collection****. Click the ****Select collections**** button and check the box in the list. If there are such products with this title they will be automatically tagged and added to the appropriate collection with the similar products.

![](https://cdn.heymantle.com/docs/screenshots/8a6c440b-f28e-4fe4-afbb-5449c83fb8cf/add-product-to-collection_d7g61e.png)

### Type

4.  We can do the same things for the product type. Select the ****Product type**** condition → set the necessary type that is in your store (in our case, we set "ring")
5.  Add the "ring" product tag
6.  Add it to the collection that contains similar products

![](https://cdn.heymantle.com/docs/screenshots/ef0d9bb5-3237-4c03-9c45-d63e52b612e7/add-product-to-collection-by-t_1udmx82.png)

## Tag orders that contain products with specific tags

If you need to detect the orders with specific products (e.g., you want to track the frequency of orders for a certain product), you can do this by tagging the orders that contain particular product tags.

1.  Select the ****Order created**** trigger
2.  Set the condition that verifies if there is a product tag → Select the ****Tag**** condition → set \*\*Any of \*\* "jeans" and "shirt"
3.  Add a necessary tag to this order

![](https://cdn.heymantle.com/docs/screenshots/70b41d57-8df4-4035-acb5-9d6ff87b7332/add-orders-tag_pzdr18.png)

## Delete the product that is out of stock and create a redirect

When a product is out of stock, we can delete it and redirect our customer to the store page with the similar product.

1.  So, add the ****Product added to store**** trigger
2.  Next, set the ****Product type**** condition → is equal to the necessary product type
3.  Set a delay of 14 days
4.  ****Create a redirect URL**** to direct customer to another store page
5.  ****Hide**** this product from the store

![](https://cdn.heymantle.com/docs/screenshots/ea8b207a-a74a-4867-b99e-976e6fb4d1a4/hide-product-by-type_1f0gd5c.png)

## Automatically set product metafield when it is added to store

To save the time, we can add a metafield to a new product and it will be automatically set to each new product with the necessary type.

1.  Start with the ****Product added to store**** trigger
2.  Verify its product type
3.  Add the necessary metafield to this product

![](https://cdn.heymantle.com/docs/screenshots/902fd968-304d-43b1-a86d-e1ab25933064/set-product-metafield_ymf07d.png)

## Suggested articles

*   [Most popular flows](/most-popular-flows)
*   [Order workflows](/order-workflows)
*   [Customer workflows](/customer-workflows)

Updated on: 25/03/2026