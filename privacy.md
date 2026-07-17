# zQinta — Privacy Policy

_Last updated: July 17, 2026_

The short version: **your knowledge stays on your Mac, and we don't see it.**

zQinta ("the app," "we," "us") is a local-first macOS application, distributed directly from our website at [zqinta.com](https://www.zqinta.com).

---

## 1. What we collect

The app is **local-first**: your knowledge maps, notes, AI chats, and API keys live **on your Mac**, and we do not see them. We run no analytics servers inside the app, no trackers, and no advertising SDKs.

The only situations in which information reaches our servers are:

- **When you register an account** (email + hashed password) — needed for the Market (buy/sell courses) and community features.
- **Community content** you choose to publish (discussions, comments) — public by design; you control what you post.
- **Payment metadata** (Stripe customer/subscription IDs, Connect account status) — we store references only. **We never see your card number** — Stripe handles all card data under their own PCI-DSS compliance.
- **Transactional emails** (account confirmation, password reset, optional notifications) — delivered via Mailgun.
- **When you email us for support** — you choose what to share (see §6).

We do **not** sell or share your personal data.

---

## 2. Where your data lives

- **Your knowledge maps** (concepts, notes, chat history) are **stored locally on your Mac.** They do not leave your device unless you explicitly export or sync them.
- **Personal notes** you add to concepts are private and are never sent to any AI model.
- **Your AI provider API keys** are stored in the **macOS Keychain** and are never sent to us.
- **Account + community data** lives on our servers (PostgreSQL) — only what's needed for login, the Market, and discussions.

---

## 3. Sync (Premium, optional)

If you subscribe to Premium and enable sync, your knowledge maps sync across your Macs via **Apple iCloud** using CloudKit's **Private Database**:

- The data is stored in **your** iCloud account, hosted and encrypted by Apple.
- It is encrypted in transit and at rest by Apple. With **iCloud Advanced Data Protection** enabled on your account, it is end-to-end encrypted.
- We (the developer) cannot read your synced data.

---

## 4. Artificial intelligence

zQinta uses AI to build your concept trees and generate video, audio, and text. How your content is processed depends on the AI source:

- **Apple on-device models** run **locally on your Mac** — no network traffic, no data leaves your device.
- **Apple Private Cloud Compute (PCC)** — for heavier reasoning, requests may be sent to Apple's PCC. Apple designs PCC so that request data is **not stored** and is **not accessible** to Apple or to us. See [Apple's privacy overview](https://www.apple.com/privacy/).
- **Bring Your Own Key (OpenAI / Anthropic / Seedance)** — if you add your own API key, the app sends your prompts **directly to that provider** over HTTPS, governed by that provider's privacy policy. Your API key is stored in the **macOS Keychain** and is never sent to us.

When you ask the AI to expand a concept or generate a lesson, the relevant concept text is included in the request so the model has context.

---

## 5. The Market (buy & sell courses)

Registered users can browse, buy, and (for Premium) sell AI-generated courses on the zQinta Market:

- **Buying** a course processes payment through **Stripe**. We store only the Stripe transaction reference, never your card.
- **Selling** (Premium) uses **Stripe Connect** to route payouts to your bank. We store your Connect account status, not banking credentials.
- Imported courses become local knowledge trees on your Mac.

---

## 6. Exports & support

- **Exports** (PDF, Markdown, JSON) are generated locally and saved wherever you choose. If you share an export with us for support, treat it as personal data — share only what you're comfortable with.
- **Support emails** contain only what you choose to send us. We use them solely to respond to you and delete them when no longer needed.

---

## 7. Subscriptions & payments

Subscription billing is processed by **Stripe** (direct distribution — not the Mac App Store). We collect only the Stripe customer/subscription ID; we never see or store your card number. You can manage or cancel your subscription at any time from the app's **Subscription** tab or via the Stripe customer portal.

Product identifiers: `com.cascadeai.zqinta.premium.monthly` and `com.cascadeai.zqinta.premium.annual`.

---

## 8. Local analytics (no PII)

If analytics are collected, they are **stored only on your device**, contain **no personal information**, and can be reset or exported from the app's settings at any time. They are never transmitted to us.

---

## 9. Children

zQinta is not directed to children under 13, and we do not knowingly collect data from children.

---

## 10. Your choices & rights

- **Delete your data:** delete individual concepts or maps in the app, or remove the app's container (Finder → Go → ⌥ Library → Containers → `com.cascadeai.zqinta`).
- **Delete your account:** Settings → Privacy & Data → Delete my account. This cancels your subscription and wipes your server-side profile, posts, and notifications. An anonymous financial record is retained for tax/legal compliance.
- **Stop sync:** disable iCloud sync in the app, or turn off iCloud Drive for the app in System Settings.
- **Remove an API key:** delete it from Settings → AI Provider.
- **Manage or cancel your subscription:** in-app Subscription tab, or System Settings if billed by Apple.
- **Access & portability (GDPR/CCPA):** download all the server-side data we hold about you from Settings → Privacy & Data → Download my data.

---

## 11. How long we keep data

- Community posts & comments — until you delete them.
- Notifications — 90 days, then automatically purged.
- Session tokens — 30 days, then expire.
- Payment records — ~7 years (tax/legal retention), anonymized on account deletion.
- Diagnostics logs (on your Mac) — 7 days, then auto-cleaned.
- Your local boards — forever, until you delete or reset them on your Mac.

---

## 12. Changes to this policy

We may update this policy; the "Last updated" date above reflects the latest version.

---

## 13. Contact

Questions about your privacy? Email **[privacy@zqinta.com](mailto:privacy@zqinta.com)**.
