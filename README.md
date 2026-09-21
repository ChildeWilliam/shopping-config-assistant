# Shopping Config Assistant / 购物配置助手

> Chrome extension support and privacy documentation for **购物配置助手（Beta）**.

购物配置助手是一款 Chrome 浏览器扩展，用于在受支持的 Apple Online Store 页面中，根据用户预先保存的商品配置和配送/自取偏好，辅助完成商品选配、购物袋检查以及联系人/配送信息填写。

## Current version

- Extension version: **0.3.1 (Beta)**
- Manifest: **Chrome Manifest V3**
- Minimum Chrome version: **102**
- Supported regions: **Apple Australia** and **Apple China Mainland**
- Status: **Beta**

## What the extension does

The extension can assist with:

- selecting a configured iPhone model, colour and storage capacity;
- handling the supported product-selection flow on Apple Online Store pages;
- adding the configured product to the shopping bag;
- checking the target product and quantity before checkout;
- choosing delivery or Apple Store pickup based on the user's saved preference;
- looking up nearby Apple Store pickup locations using an Apple-provided store lookup endpoint;
- filling contact and delivery fields with information that the user explicitly saved;
- stopping when the payment-method stage is reached.

## What the extension does not do

The extension does **not**:

- enter or store credit/debit card numbers;
- collect passwords, verification codes, PINs or other authentication credentials;
- select Apple Pay, PayPal or another payment method on the user's behalf;
- submit the final purchase order automatically;
- bypass queues, CAPTCHAs, anti-bot measures or Apple security checks;
- run advertising or third-party analytics;
- sell user data.

Payment selection, payment authentication and final order submission remain the user's responsibility.

## Permissions

The extension currently requests:

- `storage` — to save the user's product configuration, delivery/pickup preference, contact details and related local settings;
- `activeTab` — to work with the active Apple Store tab after the user starts the assistant;
- host access to supported Apple domains — to operate on supported Apple Store pages and query the official Apple pickup-store endpoint.

## Data handling

Saved configuration and contact information are stored using Chrome extension storage on the user's device. The extension does not operate a developer backend for collecting this information.

When the user starts the assisted checkout flow, contact or delivery information may be inserted into Apple webpages so that Apple can process it according to Apple's own terms and privacy policy.

For full details, see the [Privacy Policy](./PRIVACY.md).

## Privacy Policy URL for Chrome Web Store

Public GitHub version:

https://github.com/ChildeWilliam/shopping-config-assistant/blob/main/PRIVACY.md

GitHub Pages version (after Pages is enabled for the `docs/` folder):

https://childewilliam.github.io/shopping-config-assistant/privacy-policy.html

## Support

For product-support information and known limitations, see [SUPPORT.md](./SUPPORT.md).

For security-related guidance, see [SECURITY.md](./SECURITY.md).

## Important limitations

This project is currently a beta. Apple may change page structure, wording, checkout controls, address validation, pickup flow or product availability at any time. If the extension cannot identify a step safely, it is designed to stop and require manual handling rather than guess.

The extension is not an inventory reservation service and does not guarantee successful checkout, stock availability or order completion.

## Independence notice

This project is an independent browser extension and is **not affiliated with, endorsed by, sponsored by, or operated by Apple Inc.**

Apple, Apple Store, iPhone, AppleCare and Apple Pay are trademarks of Apple Inc. Their use here is solely to describe compatibility and functionality.

## Public repository scope

This public repository is used for public-facing privacy, support and Chrome Web Store documentation. It does not currently contain the full extension source code.

---

**Last documentation update:** 21 September 2026
