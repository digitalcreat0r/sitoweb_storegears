---
layout: document
title: Privacy Policy - PigeonTweak
permalink: /policies/privacy-policy-pigeontweak.html
back_url: /
back_text: Back to Home
---
# Privacy Policy - PigeonTweak

*Last updated: November 24, 2026*

**PigeonTweak** is an application for Shopify merchants, developed and managed by **{{ site.author }}** ("the developer"), operating as **{{ site.brand }}**. It lets a signed-in customer correct the shipping address on an order from the order status page or the thank-you page, while your edit window is still open and the order can still be changed. The country on the address stays the same. This policy explains what data the app accesses, why, and how long it is kept.

## 1. Who is responsible for the data
For store data and for customer data that PigeonTweak reads or updates in your Shopify store (a customer's name, shipping address, and phone number on an order), you (the merchant) are the data controller. The developer acts as a data processor and handles that data only to provide the service you installed.

For contact and support data (for example, when you email us), the data controller is **{{ site.author }} ({{ site.brand }})**, {{ site.email }}.

## 2. Data the app accesses
PigeonTweak processes customer data only so that a customer who owns an order can correct its shipping address, and so you can be told that the address changed. It does not build a customer list and does not read customer email addresses.

When you install the app, you grant these access scopes:

- **`read_orders`:** Reads the order the customer is viewing: order name and id, status, creation date, fulfillment status, order total, and the current shipping address (name, company, street, city, province, postal code, country, phone).
- **`write_orders`:** Saves the new shipping address on that order. The app does not change line items, discounts, or products.
- **`read_customers`:** Confirms that the signed-in customer owns the order. The app does not read email addresses, marketing preferences, or other profile data.
- **`read_merchant_managed_fulfillment_orders` and `read_third_party_fulfillment_orders`:** Check whether a fulfillment request has already been sent. If it has, the address can no longer be changed.
- **`write_app_proxy`:** Lets the order form call the app through your shop domain.

The app also reads your shop name, shop domain, store email address, and time zone. The store email is where merchant notices are sent, and the time zone is used for your quiet hours.

The signed-in customer submits the new address (name, company, street, city, province or state, postal code, and phone, depending on the fields you enable). You provide your settings in the app: whether corrections are on, the edit window, the form fields, and your email and quiet-hours preferences.

## 3. Data the app stores and for how long
- **Settings and sessions:** Kept while the app is installed. Sessions contain your shop domain, access credentials, and granted scopes. For an online staff session, they also contain the staff member's Shopify user id, name, and email.
- **Correction count:** A daily count of successful corrections (shop domain, date, number). It contains no order, name, address, or phone. Deleted after about 30 days.
- **Temporary holds:** If a correction changes the order total, the app keeps the previous address and the notice (including name and phone) for a few minutes so the customer can undo the change. Notices delayed by your quiet hours are kept until sent. Deleted once handled, and no later than 90 days.
- **Access record:** When a customer's name, address, or phone is read, saved, exported, or deleted, the app logs the shop domain, order id, action, and customer id. It does not store the name, address, or phone. Deleted after 90 days.
- **Support emails:** If you contact us, we keep your name, email, and shop domain only as long as needed to answer, unless the law requires longer.

Apart from the temporary holds, the app keeps no copy of the shipping address. It stays on the order in Shopify, which you control.

**Uninstall and privacy requests:** When you uninstall PigeonTweak, the app deletes the data it holds for your store. The access record is deleted when Shopify sends `shop/redact`, about 48 hours later. The app also handles Shopify's mandatory privacy webhooks (`customers/data_request`, `customers/redact`, and `shop/redact`).

## 4. Merchant notices and third parties
If merchant notices are on, the app emails your store email address when an address changes. The message includes the order name, the previous and new address (including name and phone), and, if the order total changed, the previous and new total.

- **Shopify:** PigeonTweak runs inside the Shopify admin and on the order status and thank-you pages. Shopify processes data under its [Privacy Policy](https://www.shopify.com/legal/privacy).
- **Resend:** Delivers merchant notices only. See the [Resend Privacy Policy](https://resend.com/legal/privacy-policy).
- **Hosting:** The app is hosted on Fly.io. Its database is a SQLite file on an encrypted volume in the United States (Chicago).

PigeonTweak does not use third-party analytics, advertising trackers, or profiling. It does not sell or share your data, or your customers' data, for marketing, and it makes no automated decisions with legal effects.

## 5. Security and international transfers
Data is stored on an encrypted volume, sent over HTTPS, and accessible only to the developer. No system is completely secure, so absolute security cannot be guaranteed. If a security incident exposes customer name, address, phone, or order data, the developer contains it, notifies Shopify at [security@shopify.com](mailto:security@shopify.com) within 24 hours, and notifies affected merchants as required by law.

Data may be processed outside your country, including in the United States and outside the European Economic Area. Where this happens, appropriate safeguards (such as Standard Contractual Clauses) are applied as required by law.

## 6. Your rights
Under the GDPR, the UK GDPR, the CCPA/CPRA, and other applicable laws, you have the right to access, correct, delete, restrict, or export your data and to object to its processing. You can also lodge a complaint with your local data protection authority.

- **Your store data:** Change your settings in the app at any time, or uninstall the app to delete your data. Contact us for other requests.
- **Your customers' data:** You are the data controller, so a customer should contact your store about an order. You can also write to us with your shop domain.

We answer requests within 30 days. PigeonTweak is a business tool and is not directed at children.

## 7. Changes and contact
This policy may be updated from time to time. The "Last updated" date shows the latest revision. Significant changes will be communicated through the app or by email.

Questions about your privacy: **{{ site.email }}**
