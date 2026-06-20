# Privacy Policy — Browser Health Dashboard

**Effective date:** 20 June 2026

Browser Health Dashboard ("the extension") is built to respect your privacy. This
policy explains exactly what data the extension touches, where it goes, and what it
never does.

## Short version
- **Your browsing data stays on your device.** Tab info, settings, the health-score
  history, saved sessions, and your block list are stored locally in your browser
  (`chrome.storage`). We do not have a server that receives them, and we never sell
  or share them.
- The only times data leaves your device are: (1) when you run an internet **speed
  test**, and (2) when you choose to **subscribe to Pro**. Both are described below.

## What the extension stores locally (on your device only)
- Open-tab counts/titles/URLs used to show stats and find tabs (read live, not sent
  anywhere).
- System RAM/CPU samples used for the gauges, badge, and history graph.
- Per-tab last-active timestamps used for "stale tab" detection and auto-suspend.
- Your settings (auto-suspend preferences, scheduled speed test).
- Saved sessions you create.
- Your site block list.

This information is kept in `chrome.storage` on your computer. It is not transmitted
to us and there is no account or cloud sync.

## When data leaves your device
1. **Internet speed test.** When you run a speed test (or, on Pro, when a scheduled
   test runs), the extension downloads/uploads test data to Cloudflare's public
   speed-test endpoint (`speed.cloudflare.com`). As with any web request, Cloudflare
   receives your IP address and connection metadata. We do not receive or store the
   results on any server — they are shown to you and kept locally. See Cloudflare's
   privacy policy for how they handle requests.
2. **Pro subscription (optional).** Payments are handled by **ExtensionPay** and
   **Stripe**. If you subscribe, you provide your email and payment details directly
   to them; we never see or store your card information. ExtensionPay stores your
   email and subscription status so the extension can verify whether Pro is active.
   See ExtensionPay's and Stripe's privacy policies for details.

## What we do NOT do
- We do **not** collect or transmit your browsing history. (The extension does not
  request the browsing-history permission.)
- We do **not** use analytics or tracking SDKs.
- We do **not** sell, rent, or share your data with advertisers.
- We do **not** run a server that receives your tabs, usage, or block list.

## Site blocking
The block list you create is used only to block those sites in your own browser,
via Chrome's declarativeNetRequest API. The list stays on your device.

## Permissions and why they're used
- `tabs` / `tabGroups` — tab stats, search, duplicate/stale detection, auto-suspend.
- `system.cpu` / `system.memory` — show RAM/CPU usage and the health score.
- `storage` — save your settings, history, sessions, and block list locally.
- `alarms` — periodically sample system stats and run scheduled speed tests.
- `declarativeNetRequest` — block the sites on your block list.
- Host access to `speed.cloudflare.com` — run the speed test.
- Host access to `extensionpay.com` — verify your Pro subscription status.

## Data retention & deletion
All local data lives in your browser. Removing the extension deletes it. You can
also clear individual items in the popup (remove sessions, unblock sites, etc.). To
delete your ExtensionPay subscription data, cancel your subscription and contact
ExtensionPay.

## Children
The extension is not directed to children under 13.

## Changes
We may update this policy; the "Effective date" above will change accordingly.

## Contact
Questions about this policy? Contact: **atanas_sd@abv.bg**

---
*Host this file at a public URL (e.g. GitHub Pages, a Google Site, or a Notion page)
and paste that URL into the Chrome Web Store "Privacy" field.*
