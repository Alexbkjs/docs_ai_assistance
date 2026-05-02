---
type: page
title: Integration with Weglot
seoTitle: Integration with Weglot
seoDescription: How to integrate Weglot and Selecty
slug: integration-with-weglot
order: 12
status: published
---


# Integration with Weglot

Before proceeding, we strongly recommend coordinating with the support teams of both applications. This will make the integration process smoother and faster.

## How to Integrate Weglot and the app

There are two possible setup variants:

*   Variant 1: **/nl** - language code only
*   Variant 2: **/en-nl** - language + country code (or a custom shortcut, depending on your Weglot configuration)

### Step 1: Unpublish non-default languages in Shopify

When using Weglot, all languages and translations are controlled by Weglot. You must unpublish non-default languages in Shopify.

1.  Go to the Shopify admin → **Settings** → **Languages**.
2.  **Unpublish** all languages except the default one.

![](https://cdn.heymantle.com/docs/screenshots/2a919e84-7469-467a-a4a2-d665279f06d1/unpublish-languages_q2j8s2.png)

### Step 2: Enable subdomains or subdirectories in Weglot

1.  Open the Weglot app and go to the **Projects** section.
2.  Click **Settings** → **Setup**.
3.  Enable the **Subdomains/Subdirectories** option.

![](https://cdn.heymantle.com/docs/screenshots/e29d16a5-4da6-40a4-a19a-2bfd78e16a0c/enable-subdomains-subdirectori_v77gvl.png)

### Step 3 (Optional): Add Markets in Shopify

This step is required for **Variant 2** only.

You need to create subdirectories for the default language in Shopify (for example, /en-nl) to match the subfolder structure used by Weglot. Since the default language is managed through Shopify, add resources through Shopify markets.

Note: The Weglot Advanced plan is recommended for this step, as it allows adding custom resources in Weglot.

1.  In your **Shopify admin**, go to **Settings** → **Markets**.
2.  Select the market you need.
3.  Click the + icon next to the **Domain language** option → select **New subfolder**.

![](https://cdn.heymantle.com/docs/screenshots/100ebd39-365c-49aa-9c85-0282a223ec75/domain-language_1sr5nxc.png)

4.  Manually enter the appropriate value in the **Domain Suffix** field.
5.  Click **Done**, then **Save** at the top of the page.

### Step 4: Add resources in the app

1.  Open the app and go to the **Resources** section → click on a Resource → **Add custom resource**.

![](https://cdn.heymantle.com/docs/screenshots/3bd1fb19-44ff-4099-9d68-4c695bc59dce/custom-resource_1q064cj.png)

2.  Enter a name for the custom resource group and click **Apply**.

![](https://cdn.heymantle.com/docs/screenshots/27ceebb1-5bcb-4cc7-a923-0a914880e66d/name-of-custom-resouce_17xaf09.png)

3.  Click **Add resource** and fill in the fields using the values created in Weglot.
4.  Make sure the **Retain URL while switching** checkbox is enabled to ensure correct URL behavior.

![](https://cdn.heymantle.com/docs/screenshots/4407ced0-46a9-4f4e-8ac5-367de9f8b921/retain-url_9mqlg8.png)

5.  Click **Apply**, then **Save** at the top of the page.

### Step 5: Create a selector

1.  Go to the **dashboard** and click **Create Selector**.
2.  Choose a theme, apply the necessary customizations, and save your changes.
3.  Click **Publish** to activate the selector.

For more detailed guidance, see [Getting started](/selecty/quick-start-in-selecty-geolocation-markets).

### Step 6: Add Exclusion Rules in Weglot

When Weglot translates store content, it can also modify selector links. To prevent this, exclude the relevant elements from translation.

1.  Open Weglot and go to **Translation Exclusions**.
2.  Click **Add Rule**.
3.  Add the following files:

*   #\_selectors.json
*   #sel-form

![](https://cdn.heymantle.com/docs/screenshots/255ae41c-f771-46fa-8b32-31fcb0306c44/add-excluded-blocks_at6pc5.png)

4.  Click **Save Rule**.

## Need help?

If this feels technical, our support team can guide you through the process.

For the fastest resolution, we recommend contacting the support teams of both applications:

*   App support: [support@devit.software](mailto:support@devit.software)
*   Weglot: [Weglot Help Center](https://support.weglot.com/) or in-app support
