---
type: page
title: How does Selecty affect SEO?
seoTitle: How does Selecty affect SEO?
seoDescription: About Selecty
slug: how-does-selecty-affect-seo
order: 16
status: published
---


# The app and its impact on SEO

Google recommends avoiding automatic redirects, so we suggest using geolocation recommendations instead. For further insights into how automatic redirects interact with SEO — especially when managing multi-regional and multilingual sites — refer to Google's best practices: [Google's Managing Multi-Regional Sites](https://developers.google.com/search/docs/specialty/international/managing-multi-regional-sites#let-the-user-switch-the-page-language).

## About the app

The application was developed to help store owners **manage automatic and manual switching between languages, markets, and currencies** on their Shopify stores. It provides flexible tools like [selectors](/selecty/can-i-customize-selectors) and [recommendation banners](/selecty/recommendation-banner) that make it easy for your customers to [navigate between different localized versions of your store](https://help.devit.software/en/article/stores-syncronization-1j6f77q/).

However, it is important to understand that this is **not** an SEO optimization tool.

Shopify itself handles most of the technical SEO aspects of a multilingual or multi-market store, including:

*   Sitemap generation
*   hreflang tags for language and region-specific content
*   Canonical URLs
*   Structured data

**Important:** The application does not interfere with or enhance these SEO settings. Its role is purely functional and user-focused, aimed at improving the experience by making it easy for visitors to find their preferred language, region, or currency.

## Canonical tags and multi-domain mode

When using multi-domain setups in your Shopify store (e.g. [example.com](https://example.com), [example.fr](https://example.fr), example.de), canonical tags play a crucial role in helping search engines understand which version of a page is the primary one. This helps avoid duplicate content issues and keeps your store's SEO healthy.

**Canonical tags are not managed by this application.** They are primarily generated and controlled by your [Shopify theme](https://themes.shopify.com/). Because multi-domain functionality is a built-in Shopify feature, theme developers are expected to implement canonical logic correctly when developing or customizing themes.

**Important:** If canonical tags are not configured correctly, search engines might index the wrong version of your content or treat pages as duplicates, which can negatively affect your SEO.

## How the app can affect SEO: Automatic redirects

Automatic redirects are the only aspect of the application that might have a secondary influence on SEO.

**About automatic redirects**

The application offers automatic redirection based on a visitor's browser language or geographical location. This is intended to improve user experience by guiding visitors to the most relevant version of the store — the correct language, currency, or domain.

To avoid unintended SEO issues, the application includes bot detection mechanisms to recognize search bots. When a visitor is identified as a search bot, the application attempts to prevent the automatic redirect, ensuring that search engines can reliably crawl and index the correct version of your pages.

**Limitations of bot detection**

Modern detection algorithms cannot guarantee 100% accuracy in identifying search bots, and there is always a slight chance that some bots may be misidentified.

Because of this inherent limitation, while the impact on SEO is minimal, automated processes are not foolproof.
