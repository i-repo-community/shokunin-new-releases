---
title: Settings
parent: Supervisors (admin screen)
grand_parent: User Manual
nav_order: 7
---

[🌐 日本語](../ja/admin-settings.html)

# Settings

Configure your tenant (contract-level) settings.

- Report generation settings
- AI feature settings
- Other tenant settings

Details of each setting are provided with your contract.

## The API credentials list

The list of access keys for external system integrations now shows **only the keys you can
currently use**.

- Revoked and expired keys are hidden from the list. A checkbox, with a count, switches them
  back on.
- They are only hidden — the record remains. **Keys are never deleted**, so that the record of
  who created past reports with them is preserved.

## OpenAPI (API reference)

For customers using an external system integration, **OpenAPI** is available from
**System settings** in the sidebar. It shows the specification of the Shokunin.new API
directly in your browser.

- It appears only while you are signed in with an administrator account.
- It opens in a new tab, so the admin screen stays where it was.

Depending on your environment, it may not be shown.
