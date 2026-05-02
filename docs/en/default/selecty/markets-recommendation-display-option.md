---
type: page
title: Markets recommendation display option
seoTitle: Markets recommendation display option
seoDescription: Display when necessary
slug: markets-recommendation-display-option
order: 7
status: published
---


# Display Options

## Display when necessary

The **Display when necessary** option shows the banner only when it is relevant — when visitors change their language, currency, or country.

![](https://cdn.heymantle.com/docs/screenshots/52d31ed3-0d77-42ac-96c0-ac3d8f3d6692/display-when-necessary_au9dev.png)

When a customer **visits your store for the first time**, the banner appears as a modal window. At this point, the app determines the most suitable option based on the selected resources (languages, country, currency). Language is determined by the visitor's browser language; country and currency are determined by the visitor's location.

*   If the customer closes the banner without making a selection, the currently detected value is saved.
*   If the customer makes a selection, their chosen option is saved.

As the customer continues browsing, the app tracks this saved preference. If the customer later opens a page where the current language, market, or currency differs from what was previously saved, the **banner appears again**, showing all available options so the customer can confirm or update their preference.

When the customer updates their selection, the app immediately **saves the new preference**. The banner is displayed only when the customer's language, currency, or country changes.

## Forced recommendations

The **Forced recommendations** option **strictly directs visitors** to the automatically detected language, market, or currency.

![](https://cdn.heymantle.com/docs/screenshots/1e6c468d-f73d-436a-b907-4219159cd41b/forced-recommendations_w901de.png)

When a customer visits the store for the first time, the app **compares the current store resource with the one detected automatically**. If they do not match, a modal banner appears showing only the detected option. Even if the customer closes the banner or manually confirms the suggestion, the app always saves **only the detected resource**, not the manually selected one.

As the customer continues browsing, the app consistently enforces the detected preference. If the customer switches the resource using a selector, the app **automatically redirects them back to the detected language**, market, or currency.

This option is useful when you want to ensure visitors always see the version of the store that best matches their location.

## Remember choice

The **Remember choice** option **saves the visitor's last selected** language, market, or currency and automatically redirects them to that saved preference on future visits.

![](https://cdn.heymantle.com/docs/screenshots/65ec6031-ebe7-46bf-b5cc-be34d1c1d5e2/remember-choice_1vaue0e.png)

When a customer visits the store for the first time, the app displays a banner as a modal window. The **visitor must select** a preferred language, market, or currency. Once a selection is made, the preference is saved and the app automatically switches the visitor to it if they access the store in a different language, market, or currency in the future.

If the visitor closes the banner **without making a selection**, the app saves the resources detected during the first visit instead.

Visitors **can change their preferences** by switching resources using a selector. The new selection is saved and used for all future visits until the visitor changes it again.

## Display once

The **Display once** option **shows recommendations only once** if needed and does not display them again in the future.

![](https://cdn.heymantle.com/docs/screenshots/72c27b89-cfd2-4fc3-9ebe-0a32018e166f/display-once_g338mi.png)

When a customer visits the store for the first time, the app shows a banner if they land on the **wrong version of the website**.

**For example**, a visitor from France lands on the Italian version of the store. The banner is displayed with a recommendation to switch to the version corresponding to France.

*   If the visitor selects a resource, they will see the selected language, currency, or market. They can later change their preference using a selector, and the updated choice will be applied. The **banner will not appear again**.
*   If the customer closes the banner without making a selection, the app continues using the resources detected during the first visit. The banner will also not be shown again.

## Display for everyone

The **Display for everyone** option shows recommendations to every new visitor, regardless of their country, currency, or browser language.

![](https://cdn.heymantle.com/docs/screenshots/1ab1d808-edc8-45b6-935b-d664a46ed1dd/display-for-everyone_1svx84e.png)

**For example**, a visitor from France lands on the French version of the store. The banner is still displayed with recommendations to switch to another language, currency, or market.

If a visitor from France lands on the Italian version of the store, the banner is also displayed with the same recommendation.

When a customer visits the store for the first time, the app displays a banner as a modal window.

*   If the visitor selects a resource, they will see the selected language, currency, or market. They can later change their preference using a selector, and the updated choice will be applied. The **banner will not appear again**.
*   If the customer closes the banner without making a selection, the app continues using the resources detected during the first visit. The banner will also not be shown again.

This option is similar to **Display once**. The difference is that **Display for everyone** applies to every new visitor, regardless of their country, currency, or browser language.

## Important notes

1.  The banner — except for **Display for everyone** — is displayed only if the **visitor's resource is added to a market in the store**. For example, if a visitor from France lands on a market assigned to Germany, and France is not included in any other market, the recommendation banner will not be displayed.
2.  In the builder for all types — except **When necessary** — there is an option to **specify the time** after which the banner should reappear. This always applies without conditions for **Display for everyone**, and applies to other options when their conditions are met.
