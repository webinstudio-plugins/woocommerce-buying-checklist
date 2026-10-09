# WooCommerce preorder and vendor purchase checklist

Review the payment, hosting and update requirements with your developer before buying Webin Preorder Workspace or Webin Vendor Workspace. This guide is prepared by Webin Studio, the developer of both products.

[Open the free interactive buying worksheet](https://demo.webinstudio.co.kr/resources/woo-buying/?utm_source=github&utm_medium=community&utm_campaign=webin_first_customer_202610&utm_content=woo_developer_checklist_en_v1). It exports your open questions as a text file. Answers remain in page memory and are not submitted. The website counts page views and product-link clicks separately from worksheet answers.

## Review a vendor share after a refund

[Download the free Excel worksheet](vendor-share-review.xlsx) and read [the calculation guide](VENDOR-SHARE-REVIEW.md). It reviews one USD order line using a percentage or fixed-per-unit vendor share and cumulative net refunds. The example inputs are fictional. Tax, shipping, prior payouts and payment fees are excluded, and the result does not confirm a transfer.

## Preorders: decide how the buyer pays

- At checkout: verify the enabled gateway, cancellation and refund procedure.
- After a payment request: review the return-to-pay flow and mail delivery. A sent request does not confirm payment or inbox delivery.
- Saved payment method at release: check gateway support, account eligibility, customer authorization and separate scheduling permission.

Ordinary staging/development installations block checkout and outgoing customer messages. Review the supported payment-testing procedure before purchase. Changing an environment label does not verify payment operation. Keep provider-confirmed results separate from simulated code tests.

## Vendor operations: check payouts and paid files

PayPal payout requests require account eligibility, fees, Sandbox operation, recipient checks and separate live activation. If you pay outside the plugin, verify the transfer before recording it in the ledger. A ledger entry does not send money.

Protected paid uploads require writable private storage outside every public web root and host-specific delivery checks. Confirm the private directory, backups and actual download behavior on your host. Resolve the storage requirement before offering protected paid uploads.

## Check the maintenance requirements

- Bookings and Subscriptions integrations are excluded in these releases. If either is essential, evaluate the provider's own documentation or discuss a separate implementation before purchase.
- Gumroad and Contra editions use manual ZIP updates. Assign an update owner, retain the previous ZIP and keep a restorable backup. Test the new version before updating the live site.
- Use PHP 8.1 or later with WordPress and WooCommerce. Verify your actual theme, gateway, scheduled jobs, permissions and mail delivery; this checklist does not certify compatibility.
- Nine plugin interface/message languages are included. Merchant-entered content is not automatically translated, and the installation guide is in English.
- Hosting, payment processing and mail services have separate costs.

## Current product details

| Product | Annual update/support service | Details |
| --- | --- | --- |
| Webin Preorder Workspace | USD39/year for one site, before applicable taxes | [Gumroad](https://8819526221141.gumroad.com/l/wltygf) · [Contra](https://contra.com/products/yON5uDJK-webin-preorder-workspace-woo-commerce) |
| Webin Vendor Workspace | USD99/year for one site, before applicable taxes | [Gumroad](https://8819526221141.gumroad.com/l/cyqqdh) · [Contra](https://contra.com/products/Xz1w2Htj-webin-vendor-workspace-woo-commerce) |

Installed business features are not remotely disabled when the annual service expires. Confirm the current purchase terms on the platform you choose. Gumroad product details include a 30-day money-back guarantee; this guide does not extend that guarantee to another platform's checkout.

WP Weekly included both products in its [October 6, 2026 product news](https://thewpweekly.com/issue-310/). That mention is separate from a hands-on review or a customer result.

When comparing alternatives, read the official [WooCommerce Pre-Orders](https://woocommerce.com/document/pre-orders/) and [Product Vendors](https://woocommerce.com/document/product-vendors/) requirements.

## Notes to take to your developer

Copy [the planning sheet](PLANNING-NOTES.md) or export your answers from the interactive worksheet. Do not place passwords, payment tokens, API secrets or customer exports in a public repository issue.

Requirements checked against the published Webin worksheet on October 8, 2026. This repository contains purchase-planning documents. The paid plugin source and installation ZIPs are supplied through their product pages.