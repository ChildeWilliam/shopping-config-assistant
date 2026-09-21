# Support / 支持

## Shopping Config Assistant / 购物配置助手（Beta）

Current documented version: **0.3.1**

### Supported environments

- Google Chrome 102 or later
- Apple Australia Online Store
- Apple China Mainland Online Store

### Normal workflow

1. Open the extension settings.
2. Select the supported region and product configuration.
3. Choose delivery or Apple Store pickup.
4. Enter the contact information required for the selected flow.
5. Save the settings.
6. Open the corresponding Apple product page.
7. Start the assistant from the extension popup.
8. Complete any step that the extension explicitly asks you to handle manually.
9. When the payment-method page is reached, the extension stops and the user completes payment and the final order manually.

### The extension intentionally stops when

- login or password entry is required;
- a CAPTCHA, verification code or security challenge is shown;
- a product option cannot be identified safely;
- shopping-bag contents do not match the saved configuration;
- quantity is not exactly one when automatic checkout continuation is expected;
- AppleCare or Trade In requires a choice that should be made manually;
- a pickup date/time or other unsupported step requires manual input;
- the payment-method or final-order stage is reached.

### Data reset

Open the extension settings page and use the clear/reset option to remove saved configuration and contact information managed by the extension.

### Common troubleshooting

**The extension does nothing on a page**  
Refresh the Apple page after installing or updating the extension, then restart the assisted flow.

**A button or field is not recognized**  
Apple may have changed the page structure or wording. Stop the assistant and complete the step manually rather than repeatedly retrying an uncertain action.

**Pickup search fails**  
Check the selected region, product and postal-code format, then try again. The result depends on Apple's own store lookup endpoint and current availability.

**The extension stops before payment**  
This can be expected when the page requires manual confirmation, a security step or an unsupported control.

### Reporting a problem

When reporting an issue, include:

- extension version;
- Chrome version;
- region (AU or CN);
- the step at which it stopped;
- the exact error message shown by the extension;
- a screenshot with personal information removed.

Do **not** post names, addresses, phone numbers, email addresses, passwords, verification codes or payment details in a public issue.

Repository: https://github.com/ChildeWilliam/shopping-config-assistant

### Disclaimer

This project does not guarantee stock availability, checkout success or order completion. Apple may change its websites at any time.

This project is independent and is not affiliated with or endorsed by Apple Inc.
