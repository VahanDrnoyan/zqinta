# Knowledge Universe — Privacy Policy

_Last updated: June 15, 2026_

The short version: **your knowledge stays on your Mac, and we don't see it.**

Knowledge Universe ("the app," "we," "us") is a local-first macOS application distributed on the Mac App Store.

---

## 1. What we collect

**We do not collect personal data from you.** We do not run analytics servers, trackers, or advertising SDKs, and we do not sell or share your data.

The only situations in which information reaches us are:

- **When you email us for support** — you choose what to share (see §5).
- **Apple** processes your subscription purchase and any refund requests (see §6). We never receive your payment details.

---

## 2. Where your data lives

- **Your knowledge maps** (concepts, notes, chat history) **are stored locally on your Mac.** They do not leave your device unless you explicitly export or sync them.
- **Personal notes** you add to concepts are private and are never sent to any AI model.

---

## 3. Sync (Premium, optional)

If you subscribe to Premium and enable sync, your knowledge maps sync across your Macs via **Apple iCloud** using CloudKit's **Private Database**:

- The data is stored in **your** iCloud account, hosted and encrypted by Apple.
- It is encrypted in transit and at rest by Apple. With **iCloud Advanced Data Protection** enabled on your account, it is end-to-end encrypted.
- We (the developer) cannot read your synced data.

---

## 4. Artificial intelligence

Knowledge Universe uses AI to build and explore your concept trees. How your content is processed depends on the AI source:

- **Apple on-device models** run **locally on your Mac** — no network traffic, no data leaves your device.
- **Apple Private Cloud Compute (PCC)** — for heavier reasoning, requests may be sent to Apple's PCC. Apple designs PCC so that request data is **not stored** and is **not accessible** to Apple or to us. See [Apple's privacy overview](https://www.apple.com/privacy/).
- **Bring Your Own Key (OpenAI / Anthropic)** — if you add your own API key, the app sends your prompts **directly to that provider** over HTTPS, governed by that provider's privacy policy. Your API key is stored in the **macOS Keychain** and is never sent to us.

When you ask the AI to expand a concept, the relevant concept text is included in the request so the model has context.

---

## 5. Exports & support

- **Exports** (PDF, Markdown, JSON) are generated locally and saved wherever you choose. If you share an export with us for support, treat it as personal data — share only what you're comfortable with.
- **Support emails** contain only what you choose to send us. We use them solely to respond to you and delete them when no longer needed.

---

## 6. Subscriptions & payments

Subscription billing is processed entirely by **Apple** through the Mac App Store (StoreKit). We do not collect, store, or see your payment card or Apple account details. Refunds are handled by Apple at [reportaproblem.apple.com](https://reportaproblem.apple.com).

StoreKit product identifiers: `com.cascadeai.knowledgeuniverse.premium.monthly` and `com.cascadeai.knowledgeuniverse.premium.annual`.

---

## 7. Local analytics (no PII)

If analytics are collected, they are **stored only on your device**, contain **no personal information**, and can be reset or exported from the app's settings at any time. They are never transmitted to us.

---

## 8. Children

Knowledge Universe is not directed to children under 13, and we do not knowingly collect data from children.

---

## 9. Your choices

- **Delete your data:** delete individual concepts or maps in the app, or remove the app's container (Finder → Go → ⌥ Library → Containers → `com.cascadeai.knowledgeuniverse`).
- **Stop sync:** disable iCloud sync in the app, or turn off iCloud Drive for the app in System Settings.
- **Remove an API key:** delete it from Settings → AI Provider.
- **Manage or cancel your subscription:** System Settings → Apple ID → Subscriptions.

---

## 10. Changes to this policy

We may update this policy; the "Last updated" date above reflects the latest version.

---

## 11. Contact

Questions about privacy? Email **[v.drnoyan@gmail.com](mailto:v.drnoyan@gmail.com)**.
