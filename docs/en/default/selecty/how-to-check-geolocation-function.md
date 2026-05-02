---
type: page
title: How to check geolocation function?
seoTitle: How to check geolocation function?
seoDescription: What is a geolocation function?
slug: how-to-check-geolocation-function
order: 15
status: published
---


# Geolocation function

## What is a geolocation function?

The **geolocation function** determines the location of your store visitors and offers them the appropriate market. It can also automatically redirect them to the relevant market based on their location.

If you have different languages in different markets, [Google does not recommend](https://developers.google.com/search/docs/specialty/international/managing-multi-regional-sites#let-the-user-switch-the-page-language) using automatic redirects due to the negative effect on indexing of multilingual content. We recommend disabling all automatic redirects and using market recommendations instead.

## How to check the geolocation function

If you are located in a country that is a primary market, you will most likely not see any offers to switch to another region or currency. You need a VPN to test another region.

1.  Enable **VPN**.

To check market recommendations, change your geolocation using a VPN. A VPN establishes a protected network connection through another country, which may be assigned to a different market.

Note: If you are using a VPN browser extension (for example, [ZenMate](https://chrome.google.com/webstore/detail/free-vpn-zenmate-best-vpn/fdcgdnkidjaadafnichfpabhfomcebme)), be aware that most browser extensions are not active in incognito mode by default. When entering incognito mode, make sure the VPN is enabled. If you use a VPN outside the browser (not as an extension), it should work in any mode.

Make sure the country selected in your VPN is assigned to a different market from your primary market. You can verify your detected country after enabling the VPN, for example, on [My location](https://mylocation.org/). It is recommended to do this in incognito mode to confirm the VPN is active there as well.

2.  Open your browser in **incognito mode** and visit your store.

The app saves information about site visits to avoid showing the banner on every return visit. Incognito mode simulates a first-time visit, which is exactly what you need for testing.

*   \[How to open incognito window in Chrome\]([https://support.google.com/chrome/answer/95464?hl=en&co=GENIE.Platform%3DDesktop#:~:text=Windows%2C](https://support.google.com/chrome/answer/95464?hl=en&co=GENIE.Platform%3DDesktop#:~:text=Windows%2C) Linux%2C or Chrome OS,Press ⌘ %2B Shift %2B n)
*   [How to open incognito window in Safari](https://support.apple.com/guide/safari/browse-privately-ibrw1069/mac)

If both conditions are met, the market recommendation banner should appear when you visit the store.

If the banner does not appear and you are automatically redirected to another market, check the following:

*   Go to your store Settings → Markets → in the Other markets section, click Preferences → disable the Domain/subfolder redirection option.
*   Open the app → find the Markets redirect option → disable redirect.

After disabling redirects, close all incognito windows and open them again to repeat the test.

If you still have questions, contact our support team: [support@devit.software](mailto:support@devit.software).

## Useful links

*   [Quick start in Geolocation & Markets](/selecty/quick-start-in-selecty-geolocation-markets)
*   [How does the recommendation banner work?](https://help.devit.software/en/article/how-does-the-recommendation-banner-work-16cw9r6/)
